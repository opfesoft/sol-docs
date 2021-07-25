# gm\_subsurvey

This table contains the answers to the survey questions. It's linked to [gm\_survey](gm_survey.md).

## Structure

| Field                           | Type    | Attributes | Null | Key | Default | Extra          | Comment |
|---------------------------------|---------|------------|------|-----|---------|----------------|---------|
| [surveyId](#surveyid)           | int(10) | unsigned   | NO   | PRI | NULL    | auto_increment |         |
| [questionId](#questionid)       | int(10) | unsigned   | NO   | PRI | 0       |                |         |
| [answer](#answer)               | int(10) | unsigned   | NO   |     | 0       |                |         |
| [answerComment](#answercomment) | text    |            | NO   |     | NULL    |                |         |

## Description of the fields

### surveyId

The ID of the survey. See [gm\_survey.surveyId](gm_survey.md#surveyid)

### questionId

Ref to i'th GMSurveySurveys.dbc field (all fields in that dbc point to fields in GMSurveyQuestions.dbc)

### answer

Probably some sort of ref to GMSurveyAnswers.dbc

### answerComment

The comment of the answer.
