# multipart_form
multipart_form_step1.html sets a single variable, foo. It targets Step 2 with a POST operation.
Step 2 is a CGI script, multipart_form_step2 . This form is not required to check the requests method, but it must make sure that foo is set. It must generate an HTML page which includes a form; the form must have one hidden field, which passes the value of foo forward; it must also have one additional field, where the user can set bar. It targets Step 3 with a POST operation.
Steps 3 and 4 are similar: confirm that you have the right variables, and then generate a form which has existing variables as hidden inputs, and each adds one new variable: Step 3 adds baz and Step 4 adds fred.
Step 5 validates that all of the required variables are set, and then prints them out. It should not produce a form, just the printouts.
