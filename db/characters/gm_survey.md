# gm\_survey

## Structure

| Field                     | Type     | Attributes | Null | Key | Default | Extra          | Comment |
|---------------------------|----------|------------|------|-----|---------|----------------|---------|
| [surveyId](#surveyid)     | int(10)  | unsigned   | NO   | PRI | NULL    | auto_increment |         |
| [guid](#guid)             | int(10)  | unsigned   | NO   |     | 0       |                |         |
| [mainSurvey](#mainsurvey) | int(10)  | unsigned   | NO   |     | 0       |                |         |
| [comment](#comment)       | longtext |            | NO   |     | NULL    |                |         |
| [createTime](#createtime) | int(10)  | unsigned   | NO   |     | 0       |                |         |

## Description of the fields

### surveyId

The ID of the survey.

### guid

The GUID of the character. See [characters.guid](characters.md#guid)

### mainSurvey

GMSurveyCurrentSurvey.dbc, column 1 (all 9) ref to GMSurveySurveys.dbc

### comment

The comment of the survey.

### createTime

The time when the survey was created, in Unix time.

