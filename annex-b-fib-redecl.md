Annex B - Allow functions in block to be redeclared
===================================================

## Motivation

Web compat issues seen by multiple vendors. See
<https://github.com/tc39/ecma262/issues/320>.

Firefox has already implemented the proposed semantics here to unbreak certain
pages. See [telemetry from Firefox](https://telemetry.mozilla.org/new-pipeline/dist.html#!cumulative=0&end_date=2016-02-23&keys=__none__!__none__!__none__&max_channel_version=aurora%252F46&measure=JS_DEPRECATED_LANGUAGE_EXTENSIONS_IN_CONTENT&min_channel_version=null&product=Firefox&sanitize=1&sort_keys=submissions&start_date=2016-01-28&table=0&trim=1&use_submission_date=0).
The bucket for the value 10 is how many times Firefox has allowed, in sloppy
mode, a function in a block to be redeclared during parsing. More detailed
analysis of that data is not yet done.

## Normative changes

See <https://github.com/syg/ecma262/commit/3d6532fc413b1e0e649957ce90df0f6515ac237d>.
