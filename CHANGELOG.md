# Change Log
All enhancements and patches to cookiecutter-django will be documented in this file.
This project adheres to [Semantic Versioning](http://semver.org/).

## [2016-03-14]
### Changed
- Enforce `repo_name` as proper python module (@catherinedevlin)

## [2016-03-08]
### Changed
- Docker configuration now uses docker-compose format v2 (@aeikenberry)
- Make sure that STATIC_URL != MEDIA_URL (@cdvv7788)
- fix minor typos in project README (@menzenski)
- Updated docker docs (@jayfk)

### Added
- Added database controls for docker (@jayfk)


## [2016-03-05]
### Changed
- Update version of Django, celery, django-test-plus (@luzfcb)
- Update version of Hitch tests dependencies: jupyter_client (@luzfcb)
- Update 'now' date in cookiecutter.json (@luzfcb)
- Update the usage example in README (@luzfcb)

## [2016-03-01]
### Changed
- Update version of Django, flake8, pyflakes, pytest, factory_boy, ipdb, Werkzeug, gevent (@luzfcb)
- Update version of Hitch tests dependencies: click, hitchserve, hitchsystem, hitchtest, ipython, psutil, python-dateutil(@luzfcb)
- Update Tether (JS) version to 1.2.0 (@luzfcb)

## [2016-02-24]
### Added
- Beginning support for `py.test` (@pydanny)

### Changed
- Fixed missing div closing tag for "container" on user_list.html (@Eraldo)

## [2016-02-18]
### Changed
- The status of the registration (open or closed) is now read from the project environment instead of hardcoded in the common settings file. (@Eraldo)
- Renamed the adapter.py file to adapters.py to match the django naming convention. (@Eraldo)



## [2016-02-15]
### Changed
- In `users` app adapter, fix `is_open_for_signup` missing parameter (@oryx2)
- Fixes and improvements in Hitch tests , see [#485](https://github.com/pydanny/cookiecutter-django/pull/485) (@crdoconnor)


## [2016-02-12]
### Changed
- Fixed typo (@yunti)

## [2016-02-07]
### Changed
- In `users` app, use Django 1.9 `LoginRequiredMixin` instead of django-braces implementation (@yunti)
- Update native OS libraries of Hitch Test, because [unixpackage](https://github.com/unixpackage/unixpackage) now supports multiple versions of same Linux distribution (@crdoconnor)
- Update AngularJS version to 1.5.0 (@luzfcb)
- Update version of wheel, Pillow, django_coverage_plugin (@luzfcb)
- Update version of Hitch tests dependencies: decorator, hitchselenium, ipython, ptyprocess, selenium (@luzfcb)
- Provided options for FOSS license choices, or for private efforts, no written license (@pydanny)

## [2016-02-01]
### Changed
- Update version of Django and django-floppyforms (@luzfcb)
- Update version of Hitch tests dependencies: hitchpython and selenium (@luzfcb)

## [2016-01-30]
### Changed
- Update flake8 to 2.5.2 (@luzfcb)

## [2016-01-29]
### Changed
- Update AngularJS version to 1.4.9 (@luzfcb)
- Update jQuery version to 2.2.0 (@luzfcb)
- Update 'now' date in cookiecutter.json (@luzfcb)
- Update version of boto, celery, django_coverage_plugin, django-storages-redux, flake8, gevent, gunicorn, pep8, pytest, tox, Werkzeug (@luzfcb)
- Update version of Hitch tests dependencies: colorama, decorator, hitchpostgres, hitchpython, hitchredis, hitchselenium, hitchserve, hitchsystem, hitchtest, ipython, patool, pickleshare, psutil, python-build, requests, selenium, tblib, traitlets (@luzfcb)


## [2016-01-26]
### Changed
- Fixed NEW_RELIC_APP_NAME environment variable (@jayfk)

## [2016-1-18]
### Added
- Added .dockerignore file (@bogdal)
- Docker tests for travis (@jayfk)

### Changed
- Removed the $-sign from allowed chars to generate the secret key (@jayfk)

## [2016-01-17]
### Added
- Adding a section on third party articles referencing `cookiecutter-django` (@mjheo)

### Changed
- Add celerybeat db to gitignore (@originell)

## [2016-01-16]
### Added
- Adding an explanation for having `django.contrib.sites`. (@pydanny)


## [2016-01-13]
### Changed
- Update setup.py version to 1.9.1 to match Django version. (@Collederas)
- Require Wheel 0.26.0. Needed to install certain packages on CPython 3.5+ like Pillow and psycopg2 (@audreyr)

## [2016-01-09]
### Changed
- Upgraded django-extensions to 1.6.1 as it fixes a [JSONField bug](https://github.com/django-extensions/django-extensions/blob/master/CHANGELOG.md#161) (@burhan)
- Upgraded Pillow to version 3.1.0 ([upstream changelog](https://github.com/python-pillow/Pillow/blob/master/CHANGES.rst#310-2016-01-04)) (@burhan)
- Upgraded django to 1.9.1 to integrate various [bugfixes](https://docs.djangoproject.com/en/1.9/releases/1.9.1/) (@burhan)
- Upgraded django-crispy-forms to 1.6 for [BS4 and django 1.9 compatibility fixes](https://github.com/maraujop/django-crispy-forms/blob/dev/CHANGELOG.md#160-201617) (@burhan)
- Upgraded django-model-utils to 2.4, to enable [support for django 1.9](https://github.com/carljm/django-model-utils/blob/master/CHANGES.rst#24-2015-12-03) (@burhan)

## [2016-01-08]
### Changed
- Fixed redis url on docker (@jayfk)
- Fixed docker on windows (@burhan)

## [2016-01-06]
### Added
- You can now enable or disable user registration using the ACCOUNT_ALLOW_REGISTRATION setting. (@ddiazpinto)

### Changed
- Use Postgres 9.5 on docker (@jayfk)

## [2016-01-04]
### Added
- Add Tether.js because [is needed](http://v4-alpha.getbootstrap.com/components/tooltips/#overview) for proper positioning of Bootstrap tooltips (@EricZaporzan)

### Changed
- Minor fixes in the docker documentation (@jayfk)
- Made @burhan a core committer (@pydanny)

## [2015-12-30]
### Changed
- Fixed a bug where the navbar was not displayed correctly (@jvanbrug)

## [2015-12-21]
### Changed
- Added sentry logger to celery config (@jayfk)

## [2015-12-16]
- Update preview 4xx error pages to accept `exception` argument (@theskumar)

## [2015-12-15]
### Changed
- Fix celery worker app name in Procfile (@stepmr)

## [2015-12-13]
### Changed
- Bumped Django to 1.9 (@areski)
- Support opbeat logging with celery (@stepmr)
- Update runtime.txt with PY2 support (@stepmr)

## [2015-12-12]
### Added
- Celery worker to Heroku procfile (@stepmr)

## [2015-12-11]
### Changed
- Fixed issue #436 - cookiecutter variable name was renamed from `celery_support` to `use_celery` in `tests/engine.py` (@luzfcb @otakucode)
- Updated Heroku runtime.txt for python 3.5.1 (@yunti)

## [2015-12-06]
### Changed
- Reorganization of contributors (@burhan)

## [2015-12-01]
### Changed
- Update documentation to include the installation os dependencies before development requirements (@failsafe86)

## [2015-11-29]
### Changed
- Update version of click and python-build (@luzfcb)

## [2015-11-25]
### Changed
- Update version of psutil, ipython (@luzfcb)
- Update version of gunicorn (@audreyr)
- Remove debugging tools from non-generated part of cookiecutter-django, since those are personal prefs (@audreyr)
- Update version of Django in setup.py (@luzfcb)

## [2015-11-24]
### Changed
- Update version of Django, coverage and click (@luzfcb)
- Fixed configuration for Celery in local.py. (@luzfcb @hackebrot)

## [2015-11-23]
### Changed
- Update AngularJS version to 1.4.8 (@luzfcb)
- Update version of cookiecutter, pytest, tox, whitenoise, django-test-plus, django_coverage_plugin, Werkzeug, hitchserve, tornado, unixpackage (@luzfcb)
- Update 'now' date in cookiecutter.json (@luzfcb)
- `sh` package version pinned to `1.11` (@luzfcb)

## [2015-11-22]
### Changed
- Move div class unquote outside the django if tag (@jvanbrug)
- Changed gevent to `1.1rc1` for python 3 users (@jondelmil / @jayfk)

## [2015-11-20]
### Changed
- Using python 3.5 on Heroku/Travis (@bogdal)
- Fixed typo in README (@tedmiston)

## [2015-11-18]
### Added
- Mailhog as a replacement for Maildump (@keybits)

### Removed
- Maildump because it didn't support Python 3 (@keybits)

## [2015-11-17]
### Added
- initial configuration to support opbeat (@burhan)

### Removed
- Took `*.pyc` out of .gitignore, because it's already covered by `*.py[cod]` (@audreyr)

## [2015-11-16]
### Changed
- Cleanup of main README (@burhan)

## [2015-11-15]
### Added
- Added `UserFactory` for users.User tests (@ad-m)

## [2015-11-12]
### Changed
- Update version of django-allauth (@yunti)
- Added a warning in README.rst: ```repo_name must be a valid Python module``` @cdvv7788

### Removed
- remove ```{% load url from future %}``` in templates - deprecated in django 1.9 (@yunti)

## [2015-11-11]
### Added
- Added django_coverage_plugin to measure Django template coverage (@audreyr)

## [2015-11-09]
### Changed
- Now using py.test for our test suite!! (@hackebrot)
- Python version in travis.yml is now correct for the selected version of Django (@show0k)

## [2015-11-08]
### Changed
- bump django-extensions version (@garrypolley)

## [2015-11-07]
### Added
- newrelic support (@amjith)
- DJANGO_SENTRY_DSN to env.example (@jayfk)

### Changed
- Made `post_gen_hook.set_secret_key()` only changes one CHANGEME!!! at a time. (@pydanny)
- Fixed an error where celery couldn't load the sentry DSN from settings (@jayfk)
- Renamed ADMIN_URL to DJANGO_ADMIN_URL in env.example (@ChrisPappalardo)

## [2015-11-06]
### Added
- \*tests\* to `.coveragerc`, because including it is cheating! (@pydanny)
- Binaryornot to cookiecutter-django's own tests because otherwise Python 3 blows up (@audreyr)

### Changed
- `.travis.yml` configuration to support Python 3.4 and 3.5 (@pydanny)
- `.gitignore` configuration so py.test cache files don't show up in git status.

## [2015-11-05]
### Changed
- Update version of django-extensions (@luzfcb)
- Fix gevent requirement for Python 3 (@mcho421)

## [2015-11-04]
### Changed
- Update version of Django, cookiecutter, celery, coverage, django-mailgun, django-redis, factory_boy, flake8, pytest and pytz (@luzfcb)
- Update AngularJS version to 1.4.7 (@luzfcb)
- Update 'now' date in cookiecutter.json (@luzfcb)

## [2015-10-28]
### Changed
- Update deployment-on-heroku.rst for ADMIN_URL (@yunti)

## [2015-10-27]
### Added
- Added sudo: true to the travis file (@MathijsHoogland)

## [2015-10-25]
### Added
- Move current logging config into production.py since it's not useful locally anyway. Used only if not using Sentry. (@audreyr)
- `setup.py` so we can list it on PyPI and therefore displayed on djangopackages.com as compatible with Python 3. (@pydanny)
- Versioning and tagging policy (@pydanny)
- Fixed flake8 issue (@pydanny)

## [2015-10-24]
### Changed
- Update nav in base template to latest Bootstrap 4 version (@audreyr)
- Replaced ADD with COPY in dockerfiles (@audreyr)
- Simplified development dockerfile (@jayfk)
- Moved the docker postgres volume on the development environment to it's own subfolder (@jayfk)
- Renamed DJANGO_CACHE_URL to REDIS_URL (@jayfk / proposed by @pydanny)

## [2015-10-22]
### Removed
- Remove unnecessary .gitkeep in static/images/ (@audreyr)

## [2015-10-21]
### Changed
- Updated requirements (@theskumar)
### Removed
- editorconfig comment that was just a isort settings link (@pydanny)

## [2015-10-19]
### Changed
- On Windows, don't install psycopg2 locally. Still install it in test/prod which are assumed to be Unix. (@audreyr)

## [2015-10-15]
### Changed
- Made `post_gen_hook` function to change secret keys in files more generic (@pydanny)
- Set cryptographically randomized value to `DJANGO_SECRET_KEY` in `env.example` (@pydanny)

## [2015-10-14]
### Added
- Documention of project options (@audreyr)
### Changed
- Added clarification on building for local or production (@MathijsHoogland)
- Whitespace correction in dev.yml (@MathijsHoogland)

## [2015-10-13]
### Changed
- Requirements update (@theskumar)

## [2015-10-11]
### Changed
- Fixed raven issue on development (#302) (@jazztpt)

## [2015-10-05]
### Changed
- Update version of Django, Pillow, hitchselenium, psutil (@luzfcb)

## [2015-10-04]
### Changed
- Remove stray closing tags and fix navbar margin in in base.html (@hairychris)
- Docker docs to be functional and more understandable (@audreyr)

## [2015-09-30]
### Changed
- Fixed Sentry logging with celery (@jayfk)
- Added pep8 and pyflakes to requirements (@jayfk)
- Fixed url() arguments in urls.py because String view arguments to url() is deprecated in django 1.9 (@siauPatrick)
- Update version of cookiecutter, coverage, django-environ, django-extensions, hitchpython, hitchselenium, hitchserve, pytest, pytz, whitenoise (@luzfcb)
- Update the usage example in README (@luzfcb)
- Update 'now' date in cookiecutter.json (@luzfcb)

## [2015-09-29]
### Changed
- Fix RST in Docker docs (@andor-pierdelacabeza)

## [2015-09-27]
### Added
- Added advice on how to persist changes with boot2docker (@jayfk)

###Changed
- Removed duplicate from `CONTRIBUTORS.rst` (@jayfk)

## [2015-09-26]
### Added
- Add .pylintrc and .pep8 (@kaidokert)

### Changed
- Move pep8 rules to setup.cfg (@audreyr)
- Better pep8 rules for exclusion (@audreyr)
- Document all linters (@audreyr)
- Sass linting and improvements to alerts (@audreyr)

## [2015-09-25]
### Changed
- django-mailgun requirement to 0.7.2 (@pydanny)
- Remove commented-out flake8 ignore rule. (@audreyr)

## [2015-09-24]
### Changed
- Add user-uploaded media dir to .gitignore (@audreyr)
- Update .editorconfig to use 2 spaces for html, css, scss, json (@audreyr)
- Have flake8 ignore node_modules dir (@audreyr)

## [2015-09-23]
### Changed
- Add workaround for django-debug-toolbar conflict with Bootstrap 4 (@audreyr)

## [2015-09-22]
### Added
- Add Python version option for deployment (@yunti)

## [2015-09-21]
### Changed
- django-mailgun-redux to django-mailgun, because @pydanny now has commit rights
### Removed
- Excess "loggers" from LOGGING setting (@siauPatrick)

## [2015-09-18]
### Changed
- Major reorganization of docs (@pydanny)
- Fix expanded navbar on mobile (@jayfk)
- Update various requirements (@audreyr)

## [2015-09-17]
### Added
- Fix for wsgi.py for Raven in dev (@yunti)

## [2015-09-15]
### Added
- whitespace to allow proper rendering of RST (@IanLee1521 )

## [2015-09-14]
### Added
- Functionality to delete taskapp if celery isn't going to be used (@pydanny)

### Removed
- Remove unused generated CSS styles (@audreyr)

### Changed
- Use Bootstrap margin utility class `m-b-lg` and remove our custom `navbar-header` class (@audreyr)
- Update Hitch requirements (@audreyr)

## [2015-09-13]
### Removed
- Styles that already exist in Bootstrap 4 (or 3) (@audreyr)

### Changed
- Fix issue #296 - change login.html to use [get_providers](https://github.com/pennersr/django-allauth/blob/master/allauth/socialaccount/templatetags/socialaccount.py#L84-L93) templatetag because ``allauth.socialaccount`` context processor now is [deprecated](http://django-allauth.readthedocs.org/en/latest/changelog.html#from-0-21-0) (@luzfcb)

## [2015-09-09]
### Added
- post_gen_hook to generate a secret key for use in locals.py. You should define your own for production (@pydanny)

## [2015-09-09]
### Added
- htmlcov to gitignore (@pydanny)

## [2015-09-04]
### Added
- Easy deploy Heroku button and app.json file (@bogdal)

## [2015-09-03]
### Added
- For security reasons, we set explicitly the list of allowed hosts (@bogdal)

## [2015-08-31]
### Removed
- Dokku in favor of docker-compose and other modern Django tools (@pydanny)

## [2015-08-30]
### Changed
- Moved from Bootstrap 3 to Bootstrap 4 (@audreyr)
- Slight Reorganization of the README docs (@pydanny)
- Dokku docs are out of the README and in the docs folder (@pydanny)
- Small improvements in ``install_python_dependencies.sh`` and ``install_os_dependencies.sh`` scripts (@luzfcb)
- Update version of django-crispy-forms, django-extensions, django-test-plus, gevent, coverage, hitchpython and hitchtest (@luzfcb)
- Update AngularJS version to 1.4.4 (@luzfcb)
- Update the usage example on README (@luzfcb)

## [2015-08-28]
### Changed
- Switched to django-mailgun-redux so mail doesn't blow up on Python 3 (@pydanny)


## [2015-08-27]
### Changed
- Grunt Updates: use libsass, add postcss (@288)

## [2015-08-20]
### Changed
- requirements files to match current dependency versions (@pydanny)

## [2015-08-18]
### Added
- Docker support and docker-compose (@jayfk)

## [2015-08-12]
### Added
- hitch for end-to-end testing functionality (@crdoconnor)

## [2015-08-09]
### Added
- test coverage, bringing it to 100% (@pydanny)

## 2015-08-08
### Added
- Gitter badge (@pydanny)
### Changed
- Refactor of cookiecutter-django render tests (@burhan)

## [2015-08-06]
### Added
- More test coverage, up to 97% (@pydanny)
- Slight optimization to celery configuration (@jayfk)

## [2015-08-05]
### Added
- Sentry support (@burhan)

### Changed
- Made the user object python 2 and 3 friendly (@pydanny)
- When using maildump, pin gevent. (@audreyr)
- Updated coverage version. (@audreyr)


## [2015-08-04]
### Added
- Better specification of migrations in .coveragerc. (@audreyr)

## [2015-08-03]
### Added
- Instructions for using coverage and generating reports (@audreyr)
- Coverage project-level config file (@audreyr)
- factory-boy package for improved testing  (@pydanny)
- Error message for duplicate usernames in `users.admin.MyUserCreationForm` (@pydanny)
- Tests on `users.admin.MyUserCreationForm` (@pydanny)

### Changed
- update django-all-auth to 0.23.0  (@pydanny)
- update django-test-plus to 1.0.7  (@pydanny)

### Removed
- Unnecessary users/forms.py module (@pydanny)

## [2015-07-30]
### Changed
- update django-floppyforms version to 1.5.2

## [2015-07-29]
### Removed
- Removed legacy permalink decorator from the users.User model. (@pydanny)

## [2015-07-27]
### Removed
- removed django-allauth template context processors because is deprecated now. see: https://github.com/pennersr/django-allauth/commit/634f4fe60e67c266aadcfba2981074f005db340c (@burhan)

### Changed
- update version of ipython, django-allauth (@luzfcb)
- update version of django-braces, django-floppyforms, django-model-utils (#287)(@burhan)

## [2015-07-21]
### Changed
- memcached is as a cache is replace with redis (#258)(@burhan)

## [2015-07-18]
### Changed
- Heroku deployment docs (@stepmr)
    - Heroku's free postgres tier is now "hobby-dev"
    - pg:backups require a scheduled time
    - add missing Mailgun API key
    - Django recommends setting the PYTHONHASHSEED environment variable to random. See: https://docs.djangoproject.com/en/1.8/howto/deployment/checklist/#python-options
    - Use openssl to generate a secure, random secret_key


## [2015-07-17]
### Added
- @models.permalink decorator to User.get_absolute_url() method

### Fixed
- Broken user_form.html (@pydanny)

## [2015-07-16]
### Added
- django-test-plus (@pydanny)
- option use maildump instead of ConsoleEmailHandler (@burhan)
- Changelog.md (@pydanny)

### Fixed
- where 'DEFAULT_FROM_EMAIL' was used to cast the value (@jayfk)

### Removed
- unnecessary header block tag and 'user:' prefix. (@pydanny)
