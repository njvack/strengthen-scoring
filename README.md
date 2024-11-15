# strengthen-scoring

Questionnaire scoring configuration files for the Strengthen project

## How to use this

This is a set of scoresheets and a multiscore configuration file for use with [scorify](https://github.com/uwmadison-chm/scorify). It expects one CSV data file per REDCap event, named as `strengthen__{event}` -- so, for example, `strengthen__scr` for the screening event.

Once you have scorify installed, you'd score the dataset with a command similar to:

```
score_multi <path_to_multiscore_config_csv> /path/to/scoresheets/score_{scoresheet}.csv /path/to/redcap_data/strengthen__{redcap_event}.csv /path/to/scored_data/{short_event}_{scoresheet}.csv
```

and that will produce one output file per row in the multiscore config file.

See the scorify documentation and `score_multi -h` for more help, email Nate Vack <njvack@wisc.edu>, or post to the [scorify discussion groups](https://github.com/uwmadison-chm/scorify/discussions).
```
```
