Script for Topaz presentation

For this presentation we're going to focus on the valuation of swing & storage options, however 
to set the scene I'm first going to give the very briefest survey of what Topaz is

*************
ASK RELEVANCE FREQUENTLY
*************

***************
PLUGGABLE MODELS - don't mention their models unless they ask. However do point out that we have multiple models, and have done work to plug them in.
***************

What is Topaz?
=============

Topaz is a real-time risk management & P&L system - reporting P&L, P&L explanation, VaR, risks & what-if analysis
It supports a wide range of trade types, and the addition of more is never a huge amount of work. While the focus is on commodities & energy, we also support FX, fixed income, freight and
even agricultural products. The reason being we wanted to avoid painting ourselves into a corner where addition of an unexpected product or trade type meant a huge redesign.

Topaz can be the system of record, or (more likely) can sit on top of existing system(s) of record, or Excel, or combinations of the two. 
A common use case when entry to the SOR could be delayed was to use the SOR for trades before today, and the traders' blotter for today's trades
- Show blotter & market data



*Show a report - e.g. build up forward option slide*

We aim for consistency, in several ways

  - The same reporting mechanism is used for all trade types. In particular the risks for complex trades and their hedges can either be combined or separated.

  - Whether running a report on a single book or portfolio, or (with the appropriate permissions) company wide - the reporting mechanism & presentation
    is the same

  - Fully versioned. So although the UI makes running using the latest data natural - under the hood there is nothing special. We keep all versions of everything,
    so any report is against specific versions of trade data, market data, reference data - even configuration settings. Thus any report is repeatable, which is essential 
    for P&L explanation


- Nothing is hidden. The data used in any calculation is always visible. No surprises

*Show valuation explanation*

*briefly show configuration*


Pluggable price processes
=========================

We've recently developed a mechanism to allow different price processes to be plugged in. Initially for swing, although planning to add gas storage v soon

Any price process has to do two things 
	- be able to calculate the implied variance of any period between any two observation dates
	- be able to generate paths consistent with those variances, given brownian motions of the correct dimension


*Describe mixed process and its calibration*

Calibration would typically use 1 or 2 years data. It could be scaled to be consistent with implied vols, however this can be dangerous

Currently doing a great deal of research on these






