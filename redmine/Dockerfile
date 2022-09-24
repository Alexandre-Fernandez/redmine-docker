FROM redmine:5.0.2-alpine

RUN apk update \
&& apk add git ruby \
&& git clone https://github.com/jgraichen/redmine_dashboard.git plugins/redmine_dashboard \
&& bundle config set --local without 'development test' \
&& git clone https://github.com/Ilogeek/redmine_issue_dynamic_edit.git plugins/redmine_issue_dynamic_edit \
&& git clone https://github.com/HugoHasenbein/redmine_tint_issues.git plugins/redmine_tint_issues
