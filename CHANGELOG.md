# Changelog
All notable changes to this project will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [Unreleased]
### Changed
- Use python 3.6 instead of python 2.7 in deploy stage of `.gitlab-ci.yml`

## [0.0.1] - 2019-08-20
### Added
- Initial release
- Improvements to the build stage in `.gitlab-ci.yml`
- Now GitLab will build the production bundle when updates are pushed to the `dev` branch
