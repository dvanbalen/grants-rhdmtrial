Payload for executing rules from Swagger
=======================

                                                                                                                                                                                                {
  "lookup": "grants-ksession",
  "commands": [ {
      "insert": {
        "object": {
          "com.examples.grant_categories.GrantApplication": {
            "dollarAmount": "150000",
            "mech_code": "Research Projects",
            "approp": "Direct-0872(HL)",
            "reimb_can": "N",
            "grant_type": "3",
            "aids_2": "B",
            "rfa_pa_number": "PA18-591",
            "strategic_category": "",
            "subcategory": "",
            "category": ""
          }
        },
        "disconnected": false,
        "out-identifier": "grant",
        "return-object": true,
        "entry-point": "DEFAULT"
      }
    },
    {
      "fire-all-rules": {
        "max": 10,
        "out-identifier": "firedActivations"
      }
    }
  ]
}
