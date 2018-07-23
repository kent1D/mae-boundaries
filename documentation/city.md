# MEAE Geo datas - Cities

| Field     | Explanation                                                  | Data type          |
| --------- | ------------------------------------------------------------ | ------------------ |
| name      | Name in the local language(s)                                | string             |
| name:fr   | Name in French                                               | string             |
| name:en   | Name in English                                              | string             |
| name:ar   | Name in Arabic                                               | string             |
| type      | Main french presence type in the city (see the related table) | string             |
| prio      | Priority (ascending)                                         | int                |
| latitude  | Latitude of the centroid of the city                         | float              |
| longitude | Longitude of the centroid of the city                        | float              |
| iso       | ISO code for the country                                     | string (2 letters) |
| capital   | "yes" if the city is the administrative capital of the country, "no" if it's not | string (yes\|no)   |
| ldir      | Label direction: better direction where to place the label towards the POI (N, NE, NW, E, W, S, SE, SW) | string\|null       |
| wikidata  | [Wikidata](https://www.wikidata.org) code                    | string             |

## Main french presence type in cities

| Type                      | Explanation                                                  | Prio (priority) |
| ------------------------- | ------------------------------------------------------------ | --------------- |
| ambassade                 | French embassy is in the city                                | 1               |
| rp                        | At least one permanent representation (towards an internation organization for example) is in the city | 2               |
| bureau                    | At least one "bureau" is in the city (only in Pyongyang and Taïpei) | 3               |
| consulat_general          | At least one french General Consulate is in the city         | 4               |
| consulat                  | At least one french consulate is in the city                 | 5               |
| institut_francais         | At least one french institute is in the city                 | 6               |
| institut_francais_antenne | At least one french institute office is in the city          | 7               |
| alliance_francaise        | At least one "Alliance française" is in the city             | 8               |
| centre_franco_xxx         | At least one mixed cultural center (eg: Centre franco-allemand) | 8               |

