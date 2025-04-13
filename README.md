# Sandwich_Attack_Simulator

This simulator aims to prevent Sandwich Attacks when swapping ETH / USDC The App aims to have the following features:

The app has the following sections and subsections, which aim to be interactive and responsive according to the parameters entered: 
Title: Sandwich Attack Simulator 
Subtitle: Understand how sandwich attacks work in DeFi trading

Parameters (section): The Parameters section should be placed on the left side of the screen.
Price Settings (subsection)

ETH / USDC ratio - My audience should be able to enter how much ETH could cost based on USDC. The minimum option they can enter is 1000 USDC per ETH, and the maximum 20 000 USDC per ETH.
Gas Cost (subsection)

Gas price - should go from 1 Gwei (minimum) to 500 Gwei (maximum).
Gas Cost - When the user enters the gas price, the gas cost should estimate how much it is since it will be related to the expense the victim will incur to swap tokens, and also the expense the attacker will incur to front and back-run.
Liquidity Pool (subsection)

Initial ETH Reserve - Should have a minimum value of 10 ETH and a maximum value of 500k ETH, where "K"= stands for thousands.
Initial USDC Reserve - Should have a minimum value of 10000 USDC and a maximum value of 10B, where "B" stands for billions.
Pool Fee - Should go from 0.1% (min) to 1% (max). There should be a section of
Victim's Trade (subsection)

Trade Amount - Minimum 0.001 ETH, maximum 100 ETH
Slippage Tolerance - Minimum 0.1%, maximum 10%.
Attack Parameters (subsection)

Front-run amount 0.001 ETH to 100 ETH.
After this section, there must be a button of "Simulate attack".
After people click on this button, the following sections should respond to the different parameters and make the calculations according to the values and procedure.

Price Impact visualization (section): This should be placed on the right side of the screen. 
The Y axis must have the initial state, after front-run, after victim trade, and after back-run parameters. For the X axis, it should show the ETH price depending on the parameter changes. 
Under this chart, there is a notice of green color. When the transaction has zero possibilities of being sandwich attacked and a notice of red color when the transaction has a potential risk of being sandwich attacked.

Liquidity Depth Chart (section): This is placed under the Price Impact Visualization section. This chart shows how liquidity is distributed around the current price. The sandwich attack targets the slippage in this zone. It should show a Buy Side on the left and a Sell Side on the right. In the middle of it, there should be a Sandwich Attack Zone rectangle with a current price line in the middle.

Attack summary (section): This section includes the victim's impact and the attacker's profit.

Victim Impact (subsection): Expected Output, Actual Output, Price Impact, Slippage Tolerance, Transaction Status.
Attacker's profit (subsection): Front-run Cost. Back-run Return. Gas Cost (Total): Front-run gas, back-run gas, and total gas. Net Profit. Roi. Profitable After Gas: (yes or no)
Under this subsection, there should be a toggle (to open and close) explaining why this attack could or couldn't be profitable for the attacker.

Detailed Transaction Breakdown (section): This section should go under the attack summary. And it has to have the following details that can be disclosed using a toggle for each subsection:
Front-run transaction (subsection): It should include the following interactive data: ETH Input, Fee, ETH After Fee, USDC Output, Calculation, New Pool Price.

Victim's transaction (subsection): It should include the following interactive data: ETH Input, Fee, ETH After Fee, Expected Output (Initial Pool), Actual Output (After Front-run), Difference, Slippage Tolerance, Transaction Status.

Back-run transaction (subsection): It should include the following interactive data: USDC Input, Fee, USDC After Fee, ETH Output, Calculation, Final Pool Price.

Mathematical breakdown (subsection): Constant Product Formula, Front-run Calculation, Price Impact Calculation, Profit Calculation.

The simulator should be a totally interactive one-page with toggles to make the Sandwich Attack concept and steps clear for my audience.
