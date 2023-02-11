# Useful grep commands
## 1. -r


`grep -r "domestic" .
./written_2/non-fiction/OUP/Abernathy/ch1.txt:The U.S. apparel and textile industries, like the clothing and other products they produce, have undergone tremendous changes over the past half century. From 1950 to 1995, domestic production of apparel doubled, while textile production, less vulnerable to imports, increased almost three times.5 Yet since World War II, shifting tastes in clothes, rising real incomes, and domestic and foreign competition within the textile and apparel industries have markedly reduced the proportion of consumer budgets expended on apparel and its upkeep (laundry and dry cleaning). In December 1963, apparel’s share of the Consumer Price Index was 10.63 percent;6 by December 1995, that percentage had fallen to 5.52 percent of average household expenditures.7
./written_2/non-fiction/OUP/Abernathy/ch1.txt:These changes are related to new technology and foreign competition. Exhortations to buy the “union label” or “Made in the U.S.A.” have done relatively little to stem the tide of clothing assembled overseas. For example, the per capita number of outerwear garments purchased in the United States increased from 14.3 to 28.7 in the period from 1967 to 1995.9 Imports, however, provided half the total in 1995, leaving domestic production with only about the same per capita number of outerwear garments as three decades earlier10—all this, even though apparel and textiles in the United States have long been characterized by special import regulation. Tariffs on their imports have remained higher than many other manufactured goods. Since the 1960s, national policymakers have sought to moderate the growth of imports, primarily through agreements with other governments. The Multi-Fiber Arrangement (MFA), a network of bilateral agreements negotiated with participating nations which became effective in 1974, established quotas for imports largely related to estimates of the growth of the U.S. domestic market. The stated purpose of the MFA was to provide for the “orderly” growth of trade in these products among countries on a negotiated basis. Advocates emphasized that “textiles and apparel offer proportionately more jobs, including entry-level positions, to less well educated, more disadvantaged groups in the United States than most other sectors of the economy.”11
./written_2/non-fiction/OUP/Abernathy/ch1.txt:As one consequence, the number of business failures among U.S. apparel manufacturers climbed from 227 in 1975 to a high of 567 in 1993.14 Not surprisingly, employment in the apparel sector during this period declined appreciably. And the U.S. Bureau of Labor Statistics projects a further reduction in the domestic apparel industry during the period 1996 to 2006 from 864,000 workers to just 714,00015—this from an industry that employed about 1.2 million employees in 1950 and reached a peak of 1.4 million employees in 1973.16
./written_2/non-fiction/OUP/Abernathy/ch1.txt:Those with a pessimistic view of domestic apparel manufacturing often assume that the high fashion end of the industry (the “top” of the fashion triangle in Figure 1.1, page 9) may be its best hope because U.S. firms can capitalize on their proximity to market. The highly acclaimed report by the MIT Commission on Industrial Productivity, Made in America, concludes:`


`grep -r "Lucayans" .
./written_2/travel_guides/berlitz2/Bahamas-History.txt:Centuries before the arrival of Columbus, a peaceful Amerindian people who called themselves the Luccucairi had settled in the Bahamas. Originally from South America, they had traveled up through the Caribbean islands, surviving by cultivating modest crops and from what they caught from sea and shore. Nothing in the experience of these gentle people could have prepared them for the arrival of the Pinta, the Niña, and the Santa Maria at San Salvador on 12 October 1492. Columbus believed that he had reached the East Indies and mistakenly called these people Indians. We know them today as the Lucayans. Columbus claimed the island and others in the Bahamas for his royal Spanish patrons, but not finding the gold and other riches he was seeking, he stayed for only two weeks before sailing towards Cuba.
./written_2/travel_guides/berlitz2/Bahamas-History.txt:The Spaniards never bothered to settle in the Bahamas, but the number of shipwrecks attest that their galleons frequently passed through the archipelago en route to and from the Caribbean, Florida, Bermuda, and their home ports. On Eleuthera the explorers dug a fresh-water well — at a spot now known as “Spanish Wells” — which was used to replenish the supplies of water on their ships before they began the long journey back to Europe with their cargoes of South American gold. As for the Lucayans, within 25 years all of them, perhaps some 30,000 people, were removed from the Bahamas to work — and die — in Spanish gold mines and on farms and pearl fisheries on Hispaniola (Haiti), Cuba, and elsewhere in the Caribbean.`
* The -r command reads and processes all files in the working directory recursively. This command is very useful as it allows us to search entire directories with grep instead of manually typing in each and every file. It also gives the file where it was found so we can easily find it. 
* Source: https://www.gnu.org/savannah-checkouts/gnu/grep/manual/grep.html


## 2. -l
`grep -rl "apparel" .
./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch6.txt
./written_2/non-fiction/OUP/Abernathy/ch7.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Abernathy/ch9.txt
./written_2/travel_guides/berlitz1/WhatToLosAngeles.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToLosAngeles.txt`


`grep -rl "domestic"
./written_2/non-fiction/OUP/Abernathy/ch1.txt
./written_2/non-fiction/OUP/Abernathy/ch14.txt
./written_2/non-fiction/OUP/Abernathy/ch15.txt
./written_2/non-fiction/OUP/Abernathy/ch2.txt
./written_2/non-fiction/OUP/Abernathy/ch3.txt
./written_2/non-fiction/OUP/Abernathy/ch8.txt
./written_2/non-fiction/OUP/Berk/CH4.txt
./written_2/non-fiction/OUP/Castro/chQ.txt
./written_2/non-fiction/OUP/Fletcher/ch1.txt
./written_2/non-fiction/OUP/Fletcher/ch10.txt
./written_2/non-fiction/OUP/Fletcher/ch2.txt
./written_2/non-fiction/OUP/Fletcher/ch5.txt
./written_2/non-fiction/OUP/Fletcher/ch6.txt
./written_2/non-fiction/OUP/Rybczynski/ch1.txt
./written_2/non-fiction/OUP/Rybczynski/ch2.txt
./written_2/non-fiction/OUP/Rybczynski/ch3.txt
./written_2/travel_guides/berlitz1/HistoryEdinburgh.txt
./written_2/travel_guides/berlitz1/HistoryFrance.txt
./written_2/travel_guides/berlitz1/HistoryIbiza.txt
./written_2/travel_guides/berlitz1/HistoryLakeDistrict.txt
./written_2/travel_guides/berlitz1/IntroEdinburgh.txt
./written_2/travel_guides/berlitz1/IntroFWI.txt
./written_2/travel_guides/berlitz1/IntroMalaysia.txt
./written_2/travel_guides/berlitz1/JungleMalaysia.txt
./written_2/travel_guides/berlitz1/WhatToEgypt.txt
./written_2/travel_guides/berlitz1/WhatToJapan.txt
./written_2/travel_guides/berlitz1/WhereToGreek.txt
./written_2/travel_guides/berlitz1/WhereToItaly.txt
./written_2/travel_guides/berlitz1/WhereToJapan.txt
./written_2/travel_guides/berlitz1/WhereToJerusalem.txt
./written_2/travel_guides/berlitz1/WhereToMalaysia.txt
./written_2/travel_guides/berlitz2/Athens-WhatToDo.txt
./written_2/travel_guides/berlitz2/Bahamas-WhereToGo.txt
./written_2/travel_guides/berlitz2/Budapest-WhatToDo.txt
./written_2/travel_guides/berlitz2/Budapest-WhereoGo.txt
./written_2/travel_guides/berlitz2/Canada-History.txt
./written_2/travel_guides/berlitz2/Canada-WhereToGo.txt
./written_2/travel_guides/berlitz2/Cancun-History.txt
./written_2/travel_guides/berlitz2/China-History.txt
./written_2/travel_guides/berlitz2/China-WhereToGo.txt
./written_2/travel_guides/berlitz2/Crete-History.txt
./written_2/travel_guides/berlitz2/Crete-WhereToGo.txt
./written_2/travel_guides/berlitz2/Cuba-WhereToGo.txt
./written_2/travel_guides/berlitz2/Poland-History.txt`
* The -l command only displays the list of file names with the specified pattern. This gives a much cleaner output if you simply care about which files have the specific pattern you are looking for. This when combined with -r can be very useful as it can search an entire directory for the pattern in a time effecient manner. 
* Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/


## 3. -c 
`grep -rc "apparel" written_2/non-fiction/OUP/Abernathy/
written_2/non-fiction/OUP/Abernathy/ch1.txt:53
written_2/non-fiction/OUP/Abernathy/ch14.txt:25
written_2/non-fiction/OUP/Abernathy/ch15.txt:36
written_2/non-fiction/OUP/Abernathy/ch2.txt:33
written_2/non-fiction/OUP/Abernathy/ch3.txt:21
written_2/non-fiction/OUP/Abernathy/ch6.txt:3
written_2/non-fiction/OUP/Abernathy/ch7.txt:14
written_2/non-fiction/OUP/Abernathy/ch8.txt:38
written_2/non-fiction/OUP/Abernathy/ch9.txt:14`


`grep -rc "domestic" written_2/non-fiction/OUP/Abernathy/
written_2/non-fiction/OUP/Abernathy/ch1.txt:7
written_2/non-fiction/OUP/Abernathy/ch14.txt:1
written_2/non-fiction/OUP/Abernathy/ch15.txt:7
written_2/non-fiction/OUP/Abernathy/ch2.txt:4
written_2/non-fiction/OUP/Abernathy/ch3.txt:1
written_2/non-fiction/OUP/Abernathy/ch6.txt:0
written_2/non-fiction/OUP/Abernathy/ch7.txt:0
written_2/non-fiction/OUP/Abernathy/ch8.txt:2
written_2/non-fiction/OUP/Abernathy/ch9.txt:0`
* The -c command prints only a count of the lines that match the given pattern. This gives a good estimate of the general frequency of the pattern in a set of files. 
* Source: https://www.geeksforgeeks.org/grep-command-in-unixlinux/


## 4. -n
`grep -n "apparel" written_2/non-fiction/OUP/Abernathy/ch6.txt
60:As Figure 6.6 shows, the safety stock needed to achieve a given customer service level is proportional to the standard deviation of the demand forecast.12 Simply put, the less certain retailers are of the demand for their product, the more safety stock they must hold to meet consumer needs. In the figure, we assume that the order-fulfillment rate equals 97 percent and the order-fulfillment lead time is three weeks. The parameter choices for the figures, although based on data from actual apparel firms, are for illustrative purposes only. By reducing order-fulfillment lead times, lean retailers are able to reduce the level of safety stock required to deal effectively with a given level of demand variation.
76:A few caveats are in order, however. According to HCTAR’s survey, the incidence of retail model stock programs increased significantly over the 1988–1992 period, from 7 percent to 16 percent of total volume shipped by the business units in our sample (see Figure 5.1, page 73). But there was a much smaller increase in the prevalence of model stock programs governed by apparel suppliers, reflecting the dominance of retailers in instigating new channel relationships as well as the reluctance of most retailers to allow suppliers to control merchandise on the shelf. As in all cases where partnerships might benefit the various parties involved, real-world considerations—who has the most power, who is responsible for instigating change, who will make the initial investments—often slow integration.
80:Ironically, replenishment capabilities would be of most value to the retailer for fashion products, but because of their short product lives and the unpredictability of demand, fashion products are typically not offered on a replenishment basis. From the apparel supplier’s perspective, that’s a good thing—at least for the time being. As the next chapter will make clear, the demands of lean retailing have already created plenty of inventory challenges for manufacturers.`


`grep -n "domestic" written_2/non-fiction/OUP/Abernathy/ch8.txt
 6:Gerber is also a major worldwide supplier of information systems for the sewing products industries. Its Product Data Management software provides users with all the information about an apparel product, including design, patterns, markers, sewing instructions, and assembly costs. This single software package can be made available through an in-house local area network or the World Wide Web. Computer data systems like this have enormous potential for the apparel industry. Private-label apparel for U.S. department and specialty stores, for instance, is generally designed in this country and produced by domestic contractors or overseas. Regardless of geographic location, it is always difficult for a contractor to know if it has the latest information on sewing patterns and other construction details. But via a network that allows contractors access, manufacturers’ headquarters can make sure that the information available is the most recent and complete. In addition, video instructions, which do not rely on spoken language, can demonstrate to foreign contractors what is acceptable and what is not.
71:The technology now exists to do mass customization, whether that involves a pair of jeans based on four measurements or a garment custom-made from a whole body scan. Five U.S. firms, including [TC]2, offer 3-D scanners, and there are at least two firms with systems that can adjust basic patterns to conform to individual body measurements. Custom clothing may therefore be financially available to a wider audience in the future, opening a new market in which domestic apparel manufacturers can compete. The general public interest in the possibilities of mass customization is evidenced by a recent article in The New York Times describing the techniques and reporting that representatives of several apparel firms expressed interest in exploring the public willingness to pay for better fitting clothing.`
* This command print out the line as well as the line number in the file which matches with the pattern. If you want to find a specfic pattern and you know which file it is in then this command makes searching for it a lot easier. Even if you run it in a whole directory, it can still be very useful but it is a very messy way of finding it. 
* https://www.geeksforgeeks.org/grep-command-in-unixlinux/
