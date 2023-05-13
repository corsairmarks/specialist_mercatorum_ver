# Overview

This mod is a compatibility patch between [Specialist Subject: Mercatorum](https://steamcommunity.com/sharedfiles/filedetails/?id=2962066593) and [Vassals Expanded and Reworked - FunEFork](https://steamcommunity.com/sharedfiles/filedetails/?id=2183551683).  Because Vassals Expanded and Reworked offers individual resource subsidy sliders, this version of a Mercatorum uses those instead of a workaround to implement its restrictions for commercial/infrastructure subsidies.

# Changes

Largely plays the same as Specialist Subject: Mercatorum, with additional compatibility for the addition agreement terms added by Vassals Expanded and Reworked: Ruler Designation, Government Restructuring, Domestic Affairs, Naming Rights, and Capital Relocation. Two custom agreement terms from Specialist Subject: Mercatorum have been removed (Monthly Commercial Dividends, Monthly Infrastructure Subsidies) in favor of the single resource sliders implemented by Vassals Expanded and Reworked.

Some code from Vassals Expanded and Reworked has been overridden in order to add the relevant restrictions for Mercatora.

## Compatibility

Built for Stellaris version 3.8 "Gemini." Not compatible with achievements.

### When to Install

This mod can be safely added to your savegame after the game has started. Because it adds gameplay objects (most notably things related to the Mercatorum subject specialization), it should not be removed during a game.

### Required Dependency Mods

* [Specialist Subject: Mercatorum](https://steamcommunity.com/sharedfiles/filedetails/?id=2962066593) adds the Mercatorum specialist subject and all of the supporting gameplay
* [Vassals Expanded and Reworked - FunEFork](https://steamcommunity.com/sharedfiles/filedetails/?id=2183551683) adds new subject agreement terms and ways to manage subjects

### Recommended Companion Mods

* [Colony Designation: Ecumenopolis Commercial](https://steamcommunity.com/sharedfiles/filedetails/?id=2597129991) adds commercial districts to ecumenopolis planets, to be further boosted by your Mercatorum subject
* [Enhanced Trade Districts and Designations](https://steamcommunity.com/sharedfiles/filedetails/?id=2641081470) enhances existing trade districts and colony designations - more jobs for more trade

## Known Issues

Overriding many types of game objects causes the game to log errors noting each override. Expect to see thirty-one (!) lines in the error.log file like these:

```
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial already exists, using the one at  file: common/agreement_terms/specialist_mercatorum_ver_agreement_term_overrides.txt line: 1
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure already exists, using the one at  file: common/agreement_terms/specialist_mercatorum_ver_agreement_term_overrides.txt line: 6
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_null already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 3
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_0 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 8
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_15 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 13
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_30 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 18
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_45 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 23
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_60 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 28
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_commercial_75 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 33
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_null already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 38
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_0 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 43
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_15 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 48
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_30 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 53
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_45 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 58
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_60 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 63
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_infrastructure_75 already exists, using the one at  file: common/agreement_term_values/specialist_mercatorum_ver_agreement_term_values_disabled.txt line: 68
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_energy already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 34
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_volatile_motes already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 130
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_minerals already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 206
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_exotic_gases already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 286
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_food already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 365
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_rare_crystals already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 452
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_alloys already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 528
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_minor_artifacts already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 603
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_consumer_goods already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 680
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: resource_subsidies_ver_research already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 756
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: subject_ver_government_allowed already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 846
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: subject_ver_capital_allowed already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 898
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: subject_can_be_integrated already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 952
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: subject_can_not_do_diplomacy already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 1030
[23:03:20][game_singleobjectdatabase.h:165]: Object with key: subject_cannot_expand already exists, using the one at  file: common/agreement_term_values/zz_specialist_mercatorum_ver_agreement_term_value_overrides.txt line: 1093
```

## Changelog

* 1.0.0 Initial version
* 1.1.0 Mark as compatible with Stellaris 3.8 "Gemini" - no script changes

## Source Code

Hosted on [GitHub](https://github.com/corsairmarks/specialist_mercatorum_ver)

### Development Notes

It is best to clone this repository into `<Stellaris User's Directory>/Paradox Interactive/Stellaris/mod`, and then make a connection to the `mod` folder via a `*.mod` file's `path` property. That will ensure the game can see the files, and also that CWTools will parse them. Also note that the README.md file exists in the `mod` directory but is symbolically linked in the root directory.