Das Netzwerk hat nach dem Codebuch (https://github.com/aupni03/SNA-Gastro/blob/main/Codebuch_Gastro_SNA.csv) folgende Attribute:

*Vertex-Attribute*
- id: Kürzel des Knotens zur eindeutigen Zuordnung
- name: Vollständiger Name des Knotens
- type: Handelt es sich um eine Person ("chef") oder ein Restaurant ("restaurant")?
- sex: Geschlecht 1 weiblich, 2 männlich, 0 ohne Geschlecht (bei Restaurants)
- michelin_rating: Aktuelle Bewertung im Guide Michelin nach Anzahl Sternen (1,2 oder 3)
- nationality: Herkunftsland eines Kochs oder einer Köchin
- county: Bundesland, in dem sich das Restaurant befindet
- alive: Noch am Leben 1, nicht mehr am Leben 2

Wichtig ist hierbei anzumerken, dass nicht alle Vertex-Attribute im vorliegenden two-Mode-Netzwerk auf alle Knoten anzuwenden sind. So sind die Attribute "nationality" und "alive" exklusiv für Köche, das Attribut "county" wurde nur bei Restaurants erhoben.

*Edge-Attribute*
- relationship: Welche Art von Beziehung besteht zwischen den Knoten? Lehrmeister 1, Vorgesetzter 2, Küchenchef 3, Ausbildungsort 4, Restaurantbesitz 5, Angestellt bei einem Küchenchef 6
- time: Wann hat die Beziehung begonnen? (Codiert als Jahreszahlen, z.B. 2004)
- end: Wann hat die Beziehung geendet? (Codiert als Jahreszahlen, "9999" bei noch nicht beendeten Beziehungen)