# Changelog

Notable changes to this project are documented in this file. The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## Unreleased

## v6.0.1 2021-06-22

Repository transferred to __purescript-contrib__.

Thank you @zaquest for authoring and donating this package.

Change the definition of `UInt` from `foreign import data UInt :: Type`
to `newtype UInt = UInt Number` and
remove the `instance Generic UInt`. We don't expect this will break
any dependent code. The `Generic` instance is no longer needed for making
class instances for types which use `UInt`.

## v6.0.0 2021-05-20

PureScript v0.14.x update.
