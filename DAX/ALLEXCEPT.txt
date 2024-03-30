--ALLEXCEPT Application
ClassKey =
VAR SalesAmount =
	CALCULATE(
		[SalesAmount],
		ALLEXCEPT(Product[Color])
	)
RETURN
	SalesAmount