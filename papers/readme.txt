xpath vs css:

xpath inconsistently implemented(no impementation for IE), worse performance

language for data extraction
Povodna motivacia: nieco, co riesi magneto - extrakcia dat z velkeho poctu webovych stranok 


   Nejspíš by se to na diplomku mohlo dát rozšířit, pokud byste se jakoby vrátil úplně na začátek a začal těmi kroky, které typicky diplomka na MFF má. Řekněme, že byste neměl hotového nic a zadáním by bylo něco jako univerzální nástroj (nebo přímo konkrétně jazyk?) pro scrapování dat. Pak byste postupoval asi takto:
    1. Analýza related work: Jak se dneska scrapuje, klasifikace přístupů, problémy např. s dynamickým obsahem stránek apod., jak se to řeší atd. Taková kapitola by pak končila nějaký přehledem otevřených problémů a vysvětlením na které se zaměříte a proč.
    2. Návrh vlastního přístupu: Vzhledem k tomu, co se dnes umí, resp. neumí (popř. co potřebuje firma) byste popsal návrh jazyka. Ale ne čistě dokumentaci, ale také např. možná jiná řešení, resp. kroky, proč ste se rozhodl zrovna takto apod.
    3. Popis Implementace interpretru jazyka: Jsou tam nějaké zajímavé algoritmy? Problémy? Ideálně pokud by to bylo možné popsat formálně v pseudokódu.
    4. Experimenty: Vlastně odkaz zpět ke kroku 1, protože je třeba ukázat (experimentálně nebo formálně, ale to je mnohem těžší, takže to první stačí) v čem je Váš přístup tedy lepší než nějaký stávající (efektivnější, zvládá složitější věci, apod.). Ideálně třeba vzít nějakou jinou implementaci nebo dvě a srovnat vlastnosti.
    5. Úplně na konec se popíše úvod (tj. motivace k čemu to je a proč), závěr (tj. shrnutí čeho bylo dosaženo) a kapitola 2, kde se vysvětlí používané pojmy. 

    V případě, že byste v rámci analýzy zjistil, že už něco chytřejšího existuje, tak by bylo třeba návrh + implementaci pro účely DP rozšířit. To rozšíření by mohlo plynout buďto z nějakých plánovaných požadavků firmy nebo něco vymyslíme.

    Takže ideálně asi začněte tou analýzou a pak bychom se sešli a pobavili se co ste zjistil a co s tím dál. Nemusíte přímo psát text práce (= kapitolu related work), ale aspoň nějaké body abyste informace nezapomněl. Ovšem vzhledem k tomu, že je to diplomka, podívejte se nejen po existujících implementacích, což ste asi dělali ve firmě, ale především po odborných článcích, jako např.
http://www.giovannigrasso.it/publications/2013--vldbj--oxpath-a-language-for-scalable-data-extraction-automation-and-crawling-the-deep-web.pdf
    (Do některých placených digitálních knihoven, jako např. ACM DL, IEEE apod. máme na fakultě koupený přístup, takže buďto ze školních počítačů nebo nalogováním přes web knihovny. Často mají ty články autoři i na svém webu zdarma.)
		
		do 13. 5. 2016
		Odevzdání diplomových prací pro letní termín státních závěrečných zkoušek
		do 28. 7. 2016
		Odevzdání bakalářských a diplomových prací pro podzimní termín státních závěrečných zkoušek
		
		
LIXTO INTRODUCTION
(R. Baumgartner, S. Flesca, and G. Gottlob. Supervised wrapper generation with
Lixto. To appear in Proc. of VLDB (Demonstration Session), 2001.)

// lixto, elog intro
5. R. Baumgartner, S. Flesca, and G. Gottlob. Visual web information extraction
with lixto. To appear in Proc. of VLDB, 2001.
 R. Baumgartner, S. Flesca, and G. Gottlob. Declarative information extraction,
web crawling and recursive wrapping with Lixto. In Proc. of LPNMR, 2001.


--> Serrano: wrapper for [Lixto elog intro] web, IN JAVASCRIPT, familiar for developrs
 --- can be fine tuned - integrated with the web, no visual wrappers, for developers only,
     can be much more precise.
		 -> is read write! add-remove commands (selectors+ math?)
		 -> for (web extension develppers) - incredibly easily deployable
		 -> procedural
		 -> semi-structured and strutured data
		 
*Matt what would it take to make serrano opensource?