ISSUE: `form.validate_on_submit()` always fails

Solve:

1.add csrf token in template

checkout quick_form

	{% import "bootstrap/wtf.html" as wtf %}
	{{ wtf.quick_form(form) }}

2.add `DataRequired()` validator to XxxField in XxxForm