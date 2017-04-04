**Motivation**

In 2011, one member of our group was working for the Mozambican Ministry of Planning and Development and was tasked with predicting government revenue from the nascent coal-mining industry. This example uses this scenario as a backdrop for creating a dynamic programming algorithm to model the optimal behaviour of mining companies starting mining operations in Mozambique.

**Background**

In the late 2000's, just over a decade after the end of a bloody civil war, surveys reported that Mozambique's Tete province was likely to hold the largest untapped coal reserves in the world. This spurred a rush by large multinational mining companies to obtain mining concessions in the region, and the government granted many prospection licences, and a few mining licences. In one of the poorest countries in the World, with an economy dominated until recently by fishing and agriculture, it seemed the country was on the verge of an economic revolution.

Of particular interest was the composition of Mozambican coal: while some of it was thermal coal, which is burned to generate electricity, a large amount was estimated to be coking coal, which is a necessary input into steel-making, by converting it to coke, and using that in turn to remove impurities from iron through chemical reactions. Coking coal is consiquently much more valuable than thermal coal, and its price was particularly high in 2011 (when this problem is set) due to the surge in demand for construction steel in China. Naturally, uncertainty exists regarding the sustainability of such high prices in the future, and commodity prices are known for being particularly volatile.

One of the biggest challenges faced by the mining sector, and by government, is that the coal deposits are located in the North-West of the country, far away from sea ports (which were in any case few in the North of the country) and with no proper access routes. For this reason, one mining company, Vale, decided to build its own 900km railway line, across Mozambique and Malawi to Nacala, where they would expand the port. The government also planned to renovate and expand the existing 600km railway line to Beira, in the center of the country. Other options were considered, but were less likely.

This means that in practice, mining companies are faced with a double constraint on their production levels: one is of their own production capacity, and another is the transport capacity to carry the coal to the ports to be exported.

Altogether, these summarise the main variables in our problem:

* There are several mines operating in Mozambique. Here we consider the main 6 mines: Ncondezi, Revobue, Zambeze, Beacon Hill, Benga and Moatize. In our problem, for simplification we assume all mines are owned by the same company.
* Two different products are extracted from coal deposits: coking coal and thermal coal.
* Coking coal is more valuable than thermal coal, and their prices are volatile and uncertain.
* There is some uncertainty regarding the actual composition of coal deposits in each mine. While geological surveys suggest a particular composition, the true composition is learned throughout the mining process and may deviate from these estimates.
* There are annual production capacity constraints for each mine, and a transport constraint on how much coal can be exported from the region overall.
