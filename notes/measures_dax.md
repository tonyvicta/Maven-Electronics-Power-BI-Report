## Total Revenue USD
 = SUMX(Sales, [Quantity] * RELATED(Products[Unit Price USD]))


## Total Orders
= DISTINCTCOUNT(Sales[Order Number])

## Average Order Value
 = DIVIDE([Total Revenue(USD)],[Total Orders])

## Average Delivery Time Days
= CALCULATE(AVERAGEX(Sales,[Delivery Date]-[Order Date]),Sales[StoreKey]=0)

## Revenue LY
=CALCULATE ( [Total Revenue(USD)], SAMEPERIODLASTYEAR ( DimDate[Date] ) )

## Revenue Var
= [Total Revenue(USD)] - [Revenue LY]

## Revenue Var %
= VAR LY = [Revenue LY]
VAR TY = [Total Revenue(USD)]
RETURN
IF(
    ISBLANK(LY) || LY = 0 || ISBLANK(TY),
    BLANK(),
    DIVIDE(TY - LY, LY)
)


## Best YoY Var % 
= VAR T =
    FILTER(
        ALLSELECTED(Stores[StoreKey]),
        NOT ISBLANK([Revenue Var %])
    )
RETURN
MAXX(T, [Revenue Var %])


## Worst YoY Var % 
= VAR T =
    FILTER(
        ALLSELECTED(Stores[StoreKey]),
        NOT ISBLANK([Revenue Var %])
    )
RETURN
MINX(T, [Revenue Var %])
