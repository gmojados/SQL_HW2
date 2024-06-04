# SQL_HW2

1.) mysql> mysql> select count(name) AS 'USA: CITIES'
    -> from city
    -> where  countrycode = 'usa';
+-------------+
| USA: CITIES |
+-------------+
|         274 |
+-------------+
1 row in set (0.00 sec)

2.) mysql> select population AS ARG_POP, AVG(lifeexpectancy) AS LIFE_EXP
    -> from country
    -> where code = 'arg';
+----------+----------+
| ARG_POP  | LIFE_EXP |
+----------+----------+
| 37032000 | 75.10000 |
+----------+----------+
1 row in set (0.00 sec)

3.) mysql> select * from city
    -> where countrycode = 'phl';
+-----+-------------------------+-------------+----------------------+------------+
| ID  | Name                    | CountryCode | District             | Population |
+-----+-------------------------+-------------+----------------------+------------+
| 765 | Quezon                  | PHL         | National Capital Reg |    2173831 |
| 766 | Manila                  | PHL         | National Capital Reg |    1581082 |
| 767 | Kalookan                | PHL         | National Capital Reg |    1177604 |
| 768 | Davao                   | PHL         | Southern Mindanao    |    1147116 |
| 769 | Cebu                    | PHL         | Central Visayas      |     718821 |
| 770 | Zamboanga               | PHL         | Western Mindanao     |     601794 |
| 771 | Pasig                   | PHL         | National Capital Reg |     505058 |
| 772 | Valenzuela              | PHL         | National Capital Reg |     485433 |
| 773 | Las Piñas               | PHL         | National Capital Reg |     472780 |
| 774 | Antipolo                | PHL         | Southern Tagalog     |     470866 |
| 775 | Taguig                  | PHL         | National Capital Reg |     467375 |
| 776 | Cagayan de Oro          | PHL         | Northern Mindanao    |     461877 |
| 777 | Parañaque               | PHL         | National Capital Reg |     449811 |
| 778 | Makati                  | PHL         | National Capital Reg |     444867 |
| 779 | Bacolod                 | PHL         | Western Visayas      |     429076 |
| 780 | General Santos          | PHL         | Southern Mindanao    |     411822 |
| 781 | Marikina                | PHL         | National Capital Reg |     391170 |
| 782 | Dasmariñas              | PHL         | Southern Tagalog     |     379520 |
| 783 | Muntinlupa              | PHL         | National Capital Reg |     379310 |
| 784 | Iloilo                  | PHL         | Western Visayas      |     365820 |
| 785 | Pasay                   | PHL         | National Capital Reg |     354908 |
| 786 | Malabon                 | PHL         | National Capital Reg |     338855 |
| 787 | San José del Monte      | PHL         | Central Luzon        |     315807 |
| 788 | Bacoor                  | PHL         | Southern Tagalog     |     305699 |
| 789 | Iligan                  | PHL         | Central Mindanao     |     285061 |
| 790 | Calamba                 | PHL         | Southern Tagalog     |     281146 |
| 791 | Mandaluyong             | PHL         | National Capital Reg |     278474 |
| 792 | Butuan                  | PHL         | Caraga               |     267279 |
| 793 | Angeles                 | PHL         | Central Luzon        |     263971 |
| 794 | Tarlac                  | PHL         | Central Luzon        |     262481 |
| 795 | Mandaue                 | PHL         | Central Visayas      |     259728 |
| 796 | Baguio                  | PHL         | CAR                  |     252386 |
| 797 | Batangas                | PHL         | Southern Tagalog     |     247588 |
| 798 | Cainta                  | PHL         | Southern Tagalog     |     242511 |
| 799 | San Pedro               | PHL         | Southern Tagalog     |     231403 |
| 800 | Navotas                 | PHL         | National Capital Reg |     230403 |
| 801 | Cabanatuan              | PHL         | Central Luzon        |     222859 |
| 802 | San Fernando            | PHL         | Central Luzon        |     221857 |
| 803 | Lipa                    | PHL         | Southern Tagalog     |     218447 |
| 804 | Lapu-Lapu               | PHL         | Central Visayas      |     217019 |
| 805 | San Pablo               | PHL         | Southern Tagalog     |     207927 |
| 806 | Biñan                   | PHL         | Southern Tagalog     |     201186 |
| 807 | Taytay                  | PHL         | Southern Tagalog     |     198183 |
| 808 | Lucena                  | PHL         | Southern Tagalog     |     196075 |
| 809 | Imus                    | PHL         | Southern Tagalog     |     195482 |
| 810 | Olongapo                | PHL         | Central Luzon        |     194260 |
| 811 | Binangonan              | PHL         | Southern Tagalog     |     187691 |
| 812 | Santa Rosa              | PHL         | Southern Tagalog     |     185633 |
| 813 | Tagum                   | PHL         | Southern Mindanao    |     179531 |
| 814 | Tacloban                | PHL         | Eastern Visayas      |     178639 |
| 815 | Malolos                 | PHL         | Central Luzon        |     175291 |
| 816 | Mabalacat               | PHL         | Central Luzon        |     171045 |
| 817 | Cotabato                | PHL         | Central Mindanao     |     163849 |
| 818 | Meycauayan              | PHL         | Central Luzon        |     163037 |
| 819 | Puerto Princesa         | PHL         | Southern Tagalog     |     161912 |
| 820 | Legazpi                 | PHL         | Bicol                |     157010 |
| 821 | Silang                  | PHL         | Southern Tagalog     |     156137 |
| 822 | Ormoc                   | PHL         | Eastern Visayas      |     154297 |
| 823 | San Carlos              | PHL         | Ilocos               |     154264 |
| 824 | Kabankalan              | PHL         | Western Visayas      |     149769 |
| 825 | Talisay                 | PHL         | Central Visayas      |     148110 |
| 826 | Valencia                | PHL         | Northern Mindanao    |     147924 |
| 827 | Calbayog                | PHL         | Eastern Visayas      |     147187 |
| 828 | Santa Maria             | PHL         | Central Luzon        |     144282 |
| 829 | Pagadian                | PHL         | Western Mindanao     |     142515 |
| 830 | Cadiz                   | PHL         | Western Visayas      |     141954 |
| 831 | Bago                    | PHL         | Western Visayas      |     141721 |
| 832 | Toledo                  | PHL         | Central Visayas      |     141174 |
| 833 | Naga                    | PHL         | Bicol                |     137810 |
| 834 | San Mateo               | PHL         | Southern Tagalog     |     135603 |
| 835 | Panabo                  | PHL         | Southern Mindanao    |     133950 |
| 836 | Koronadal               | PHL         | Southern Mindanao    |     133786 |
| 837 | Marawi                  | PHL         | Central Mindanao     |     131090 |
| 838 | Dagupan                 | PHL         | Ilocos               |     130328 |
| 839 | Sagay                   | PHL         | Western Visayas      |     129765 |
| 840 | Roxas                   | PHL         | Western Visayas      |     126352 |
| 841 | Lubao                   | PHL         | Central Luzon        |     125699 |
| 842 | Digos                   | PHL         | Southern Mindanao    |     125171 |
| 843 | San Miguel              | PHL         | Central Luzon        |     123824 |
| 844 | Malaybalay              | PHL         | Northern Mindanao    |     123672 |
| 845 | Tuguegarao              | PHL         | Cagayan Valley       |     120645 |
| 846 | Ilagan                  | PHL         | Cagayan Valley       |     119990 |
| 847 | Baliuag                 | PHL         | Central Luzon        |     119675 |
| 848 | Surigao                 | PHL         | Caraga               |     118534 |
| 849 | San Carlos              | PHL         | Western Visayas      |     118259 |
| 850 | San Juan del Monte      | PHL         | National Capital Reg |     117680 |
| 851 | Tanauan                 | PHL         | Southern Tagalog     |     117539 |
| 852 | Concepcion              | PHL         | Central Luzon        |     115171 |
| 853 | Rodriguez (Montalban)   | PHL         | Southern Tagalog     |     115167 |
| 854 | Sariaya                 | PHL         | Southern Tagalog     |     114568 |
| 855 | Malasiqui               | PHL         | Ilocos               |     113190 |
| 856 | General Mariano Alvarez | PHL         | Southern Tagalog     |     112446 |
| 857 | Urdaneta                | PHL         | Ilocos               |     111582 |
| 858 | Hagonoy                 | PHL         | Central Luzon        |     111425 |
| 859 | San Jose                | PHL         | Southern Tagalog     |     111009 |
| 860 | Polomolok               | PHL         | Southern Mindanao    |     110709 |
| 861 | Santiago                | PHL         | Cagayan Valley       |     110531 |
| 862 | Tanza                   | PHL         | Southern Tagalog     |     110517 |
| 863 | Ozamis                  | PHL         | Northern Mindanao    |     110420 |
| 864 | Mexico                  | PHL         | Central Luzon        |     109481 |
| 865 | San Jose                | PHL         | Central Luzon        |     108254 |
| 866 | Silay                   | PHL         | Western Visayas      |     107722 |
| 867 | General Trias           | PHL         | Southern Tagalog     |     107691 |
| 868 | Tabaco                  | PHL         | Bicol                |     107166 |
| 869 | Cabuyao                 | PHL         | Southern Tagalog     |     106630 |
| 870 | Calapan                 | PHL         | Southern Tagalog     |     105910 |
| 871 | Mati                    | PHL         | Southern Mindanao    |     105908 |
| 872 | Midsayap                | PHL         | Central Mindanao     |     105760 |
| 873 | Cauayan                 | PHL         | Cagayan Valley       |     103952 |
| 874 | Gingoog                 | PHL         | Northern Mindanao    |     102379 |
| 875 | Dumaguete               | PHL         | Central Visayas      |     102265 |
| 876 | San Fernando            | PHL         | Ilocos               |     102082 |
| 877 | Arayat                  | PHL         | Central Luzon        |     101792 |
| 878 | Bayawan (Tulong)        | PHL         | Central Visayas      |     101391 |
| 879 | Kidapawan               | PHL         | Central Mindanao     |     101205 |
| 880 | Daraga (Locsin)         | PHL         | Bicol                |     101031 |
| 881 | Marilao                 | PHL         | Central Luzon        |     101017 |
| 882 | Malita                  | PHL         | Southern Mindanao    |     100000 |
| 883 | Dipolog                 | PHL         | Western Mindanao     |      99862 |
| 884 | Cavite                  | PHL         | Southern Tagalog     |      99367 |
| 885 | Danao                   | PHL         | Central Visayas      |      98781 |
| 886 | Bislig                  | PHL         | Caraga               |      97860 |
| 887 | Talavera                | PHL         | Central Luzon        |      97329 |
| 888 | Guagua                  | PHL         | Central Luzon        |      96858 |
| 889 | Bayambang               | PHL         | Ilocos               |      96609 |
| 890 | Nasugbu                 | PHL         | Southern Tagalog     |      96113 |
| 891 | Baybay                  | PHL         | Eastern Visayas      |      95630 |
| 892 | Capas                   | PHL         | Central Luzon        |      95219 |
| 893 | Sultan Kudarat          | PHL         | ARMM                 |      94861 |
| 894 | Laoag                   | PHL         | Ilocos               |      94466 |
| 895 | Bayugan                 | PHL         | Caraga               |      93623 |
| 896 | Malungon                | PHL         | Southern Mindanao    |      93232 |
| 897 | Santa Cruz              | PHL         | Southern Tagalog     |      92694 |
| 898 | Sorsogon                | PHL         | Bicol                |      92512 |
| 899 | Candelaria              | PHL         | Southern Tagalog     |      92429 |
| 900 | Ligao                   | PHL         | Bicol                |      90603 |
+-----+-------------------------+-------------+----------------------+------------+
136 rows in set (0.01 sec)



4.) mysql> select *
    -> from city
    -> where population < 1000;
+------+---------------------+-------------+-------------+------------+
| ID   | Name                | CountryCode | District    | Population |
+------+---------------------+-------------+-------------+------------+
|   61 | South Hill          | AIA         | –           |        961 |
|   62 | The Valley          | AIA         | –           |        595 |
| 1791 | Flying Fish Cove    | CXR         | –           |        700 |
| 2316 | Bantam              | CCK         | Home Island |        503 |
| 2317 | West Island         | CCK         | West Island |        167 |
| 2728 | Yaren               | NRU         | –           |        559 |
| 2805 | Alofi               | NIU         | –           |        682 |
| 2806 | Kingston            | NFK         | –           |        800 |
| 2912 | Adamstown           | PCN         | –           |         42 |
| 3333 | Fakaofo             | TKL         | Fakaofo     |        300 |
| 3538 | Città del Vaticano  | VAT         | –           |        455 |
+------+---------------------+-------------+-------------+------------+
11 rows in set (0.00 sec)




5.) mysql> select*
    -> from country
    -> where region like 'east___ %';
+------+--------------------------------+-----------+----------------+-------------+-----------+------------+----------------+------------+------------+----------------------------------------------+----------------------------------------+----------------------------------+---------+-------+
| Code | Name                           | Continent | Region         | SurfaceArea | IndepYear | Population | LifeExpectancy | GNP        | GNPOld     | LocalName                                    | GovernmentForm                         | HeadOfState                      | Capital | Code2 |
+------+--------------------------------+-----------+----------------+-------------+-----------+------------+----------------+------------+------------+----------------------------------------------+----------------------------------------+----------------------------------+---------+-------+
| BDI  | Burundi                        | Africa    | Eastern Africa |    27834.00 |      1962 |    6695000 |           46.2 |     903.00 |     982.00 | Burundi/Uburundi                             | Republic                               | Pierre Buyoya                    |     552 | BI    |
| BGR  | Bulgaria                       | Europe    | Eastern Europe |   110994.00 |      1908 |    8190900 |           70.9 |   12178.00 |   10169.00 | Balgarija                                    | Republic                               | Petar Stojanov                   |     539 | BG    |
| BLR  | Belarus                        | Europe    | Eastern Europe |   207600.00 |      1991 |   10236000 |           68.0 |   13714.00 |       NULL | Belarus                                      | Republic                               | Aljaksandr Lukašenka             |    3520 | BY    |
| CHN  | China                          | Asia      | Eastern Asia   |  9572900.00 |     -1523 | 1277558000 |           71.4 |  982268.00 |  917719.00 | Zhongquo                                     | People'sRepublic                       | Jiang Zemin                      |    1891 | CN    |
| COM  | Comoros                        | Africa    | Eastern Africa |     1862.00 |      1975 |     578000 |           60.0 |    4401.00 |    4361.00 | Komori/Comores                               | Republic                               | Azali Assoumani                  |    2295 | KM    |
| CZE  | Czech Republic                 | Europe    | Eastern Europe |    78866.00 |      1993 |   10278100 |           74.5 |   55017.00 |   52037.00 | ¸esko                                        | Republic                               | Václav Havel                     |    3339 | CZ    |
| DJI  | Djibouti                       | Africa    | Eastern Africa |    23200.00 |      1977 |     638000 |           50.8 |     382.00 |     373.00 | Djibouti/Jibuti                              | Republic                               | Ismail Omar Guelleh              |     585 | DJ    |
| ERI  | Eritrea                        | Africa    | Eastern Africa |   117600.00 |      1993 |    3850000 |           55.8 |     650.00 |     755.00 | Ertra                                        | Republic                               | Isayas Afewerki [Isaias Afwerki] |     652 | ER    |
| ETH  | Ethiopia                       | Africa    | Eastern Africa |  1104300.00 |     -1000 |   62565000 |           45.2 |    6353.00 |    6180.00 | YeItyop´iya                                  | Republic                               | Negasso Gidada                   |     756 | ET    |
| HKG  | Hong Kong                      | Asia      | Eastern Asia   |     1075.00 |      NULL |    6782000 |           79.5 |  166448.00 |  173610.00 | Xianggang/Hong Kong                          | Special Administrative Region of China | Jiang Zemin                      |     937 | HK    |
| HUN  | Hungary                        | Europe    | Eastern Europe |    93030.00 |      1918 |   10043200 |           71.4 |   48267.00 |   45914.00 | Magyarország                                 | Republic                               | Ferenc Mádl                      |    3483 | HU    |
| IOT  | British Indian Ocean Territory | Africa    | Eastern Africa |       78.00 |      NULL |          0 |           NULL |       0.00 |       NULL | British Indian Ocean Territory               | Dependent Territory of the UK          | Elisabeth II                     |    NULL | IO    |
| JPN  | Japan                          | Asia      | Eastern Asia   |   377829.00 |      -660 |  126714000 |           80.7 | 3787042.00 | 4192638.00 | Nihon/Nippon                                 | Constitutional Monarchy                | Akihito                          |    1532 | JP    |
| KEN  | Kenya                          | Africa    | Eastern Africa |   580367.00 |      1963 |   30080000 |           48.0 |    9217.00 |   10241.00 | Kenya                                        | Republic                               | Daniel arap Moi                  |    1881 | KE    |
| KOR  | South Korea                    | Asia      | Eastern Asia   |    99434.00 |      1948 |   46844000 |           74.4 |  320749.00 |  442544.00 | Taehan Min’guk (Namhan)                      | Republic                               | Kim Dae-jung                     |    2331 | KR    |
| MAC  | Macao                          | Asia      | Eastern Asia   |       18.00 |      NULL |     473000 |           81.6 |    5749.00 |    5940.00 | Macau/Aomen                                  | Special Administrative Region of China | Jiang Zemin                      |    2454 | MO    |
| MDA  | Moldova                        | Europe    | Eastern Europe |    33851.00 |      1991 |    4380000 |           64.5 |    1579.00 |    1872.00 | Moldova                                      | Republic                               | Vladimir Voronin                 |    2690 | MD    |
| MDG  | Madagascar                     | Africa    | Eastern Africa |   587041.00 |      1960 |   15942000 |           55.0 |    3750.00 |    3545.00 | Madagasikara/Madagascar                      | Federal Republic                       | Didier Ratsiraka                 |    2455 | MG    |
| MNG  | Mongolia                       | Asia      | Eastern Asia   |  1566500.00 |      1921 |    2662000 |           67.3 |    1043.00 |     933.00 | Mongol Uls                                   | Republic                               | Natsagiin Bagabandi              |    2696 | MN    |
| MOZ  | Mozambique                     | Africa    | Eastern Africa |   801590.00 |      1975 |   19680000 |           37.5 |    2891.00 |    2711.00 | Moçambique                                   | Republic                               | Joaquím A. Chissano              |    2698 | MZ    |
| MUS  | Mauritius                      | Africa    | Eastern Africa |     2040.00 |      1968 |    1158000 |           71.0 |    4251.00 |    4186.00 | Mauritius                                    | Republic                               | Cassam Uteem                     |    2511 | MU    |
| MWI  | Malawi                         | Africa    | Eastern Africa |   118484.00 |      1964 |   10925000 |           37.6 |    1687.00 |    2527.00 | Malawi                                       | Republic                               | Bakili Muluzi                    |    2462 | MW    |
| MYT  | Mayotte                        | Africa    | Eastern Africa |      373.00 |      NULL |     149000 |           59.5 |       0.00 |       NULL | Mayotte                                      | Territorial Collectivity of France     | Jacques Chirac                   |    2514 | YT    |
| POL  | Poland                         | Europe    | Eastern Europe |   323250.00 |      1918 |   38653600 |           73.2 |  151697.00 |  135636.00 | Polska                                       | Republic                               | Aleksander Kwasniewski           |    2928 | PL    |
| PRK  | North Korea                    | Asia      | Eastern Asia   |   120538.00 |      1948 |   24039000 |           70.7 |    5332.00 |       NULL | Choson Minjujuui In´min Konghwaguk (Bukhan)  | Socialistic Republic                   | Kim Jong-il                      |    2318 | KP    |
| REU  | Réunion                        | Africa    | Eastern Africa |     2510.00 |      NULL |     699000 |           72.7 |    8287.00 |    7988.00 | Réunion                                      | Overseas Department of France          | Jacques Chirac                   |    3017 | RE    |
| ROM  | Romania                        | Europe    | Eastern Europe |   238391.00 |      1878 |   22455500 |           69.9 |   38158.00 |   34843.00 | România                                      | Republic                               | Ion Iliescu                      |    3018 | RO    |
| RUS  | Russian Federation             | Europe    | Eastern Europe | 17075400.00 |      1991 |  146934000 |           67.2 |  276608.00 |  442989.00 | Rossija                                      | Federal Republic                       | Vladimir Putin                   |    3580 | RU    |
| RWA  | Rwanda                         | Africa    | Eastern Africa |    26338.00 |      1962 |    7733000 |           39.3 |    2036.00 |    1863.00 | Rwanda/Urwanda                               | Republic                               | Paul Kagame                      |    3047 | RW    |
| SOM  | Somalia                        | Africa    | Eastern Africa |   637657.00 |      1960 |   10097000 |           46.2 |     935.00 |       NULL | Soomaaliya                                   | Republic                               | Abdiqassim Salad Hassan          |    3214 | SO    |
| SVK  | Slovakia                       | Europe    | Eastern Europe |    49012.00 |      1993 |    5398700 |           73.7 |   20594.00 |   19452.00 | Slovensko                                    | Republic                               | Rudolf Schuster                  |    3209 | SK    |
| SYC  | Seychelles                     | Africa    | Eastern Africa |      455.00 |      1976 |      77000 |           70.4 |     536.00 |     539.00 | Sesel/Seychelles                             | Republic                               | France-Albert René               |    3206 | SC    |
| TWN  | Taiwan                         | Asia      | Eastern Asia   |    36188.00 |      1945 |   22256000 |           76.4 |  256254.00 |  263451.00 | T’ai-wan                                     | Republic                               | Chen Shui-bian                   |    3263 | TW    |
| TZA  | Tanzania                       | Africa    | Eastern Africa |   883749.00 |      1961 |   33517000 |           52.3 |    8005.00 |    7388.00 | Tanzania                                     | Republic                               | Benjamin William Mkapa           |    3306 | TZ    |
| UGA  | Uganda                         | Africa    | Eastern Africa |   241038.00 |      1962 |   21778000 |           42.9 |    6313.00 |    6887.00 | Uganda                                       | Republic                               | Yoweri Museveni                  |    3425 | UG    |
| UKR  | Ukraine                        | Europe    | Eastern Europe |   603700.00 |      1991 |   50456000 |           66.0 |   42168.00 |   49677.00 | Ukrajina                                     | Republic                               | Leonid Kutšma                    |    3426 | UA    |
| ZMB  | Zambia                         | Africa    | Eastern Africa |   752618.00 |      1964 |    9169000 |           37.2 |    3377.00 |    3922.00 | Zambia                                       | Republic                               | Frederick Chiluba                |    3162 | ZM    |
| ZWE  | Zimbabwe                       | Africa    | Eastern Africa |   390757.00 |      1980 |   11669000 |           37.8 |    5951.00 |    8670.00 | Zimbabwe                                     | Republic                               | Robert G. Mugabe                 |    4068 | ZW    |
+------+--------------------------------+-----------+----------------+-------------+-----------+------------+----------------+------------+------------+----------------------------------------------+----------------------------------------+----------------------------------+---------+-------+
38 rows in set (0.00 sec)
