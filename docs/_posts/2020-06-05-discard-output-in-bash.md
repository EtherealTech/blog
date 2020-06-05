---
layout: master
title: Discard output in Bash
category: [bash]
tags: [bash,command,linux,unix,shell]
---

# Discard output in Bash

`> /dev/null` redirects standard output (stdout) to `/dev/null`, which discards it.

(The `>>` seems sort of superfluous, since `>>` means append while `>` means truncate and write, and either appending to or writing to `/dev/null` has the same net effect. I usually just use `>` for that reason.)

`2>&1` redirects standard error (2) to standard output (1), which then discards it as well since standard output has already been redirected.
