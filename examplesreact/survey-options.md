---
layout: example
usereact: true
propertiesFile: exampleproperties/options.html
title: Use properties to set up your survey
---
{% capture survey_setup %}
var survey = new ReactSurveyModel({% include surveys/survey-severalpages.json %});
survey.showProgressBar = "bottom";
ReactDOM.render(<ReactSurvey model={survey} />, document.getElementById("surveyElement"));
{% endcapture %}

{% include live-example-code.html %}