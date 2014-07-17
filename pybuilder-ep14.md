# Practical PyBuilder {data-background="res/pybuilder.png" data-background-size="5%" data-background-repeat="none" data-background-position="right bottom" .spaceps}

_Maximilien Riehl_

<div style="margin: 2em 1em 0em; text-align: right;">
<small>July 25th, 2014</small>
</div>

# Context TLDR{data-background="res/firmensitz.jpg" .opaque}

* I'm from a german web shop
* We love python
* We're spreading the love in our department

# cinescript test

<div
    data-typescript="demos/tmp/typescript"
    data-timing="demos/tmp/timing"
    data-autoplay="false"
    data-speed=2
    data-cols=112
    data-rows=15
    style="font-size: 20px;"
    class="cinescript">
</div>

# Sneak peek

<div
    data-typescript="demos/script-yadtshell"
    data-timing="demos/timing-yadtshell"
    data-autoplay="false"
    data-speed=2
    data-cols=112
    data-rows=15
    style="font-size: 20px;"
    class="cinescript">
</div>

# Running tasks / default tasks
Small logic building block

```bash
pyb run_unit_tests analyze
```

# It just works™

```bash
pyb
```
and in `build.py`:
```python
url = 'https://github.com/yadt/yadtshell'
version = '1.8.5'

default_task = ['clean', 'analyze', 'publish']


@init
def set_properties(project):
    project.depends_on('hostexpand')
```

# TLDR: like make, but with batteries
* flake8
* install_dependencies
* unittest
* distutils

# Get started with start-project
```bash
pyb --start-project
```

# Another term with something else entirely

<div
    data-typescript="demos/script-sl"
    data-timing="demos/timing-sl"
    data-speed=2
    data-cols=112
    data-rows=15
    style="font-size: 20px;"
    data-autoplay="false"
    class="cinescript">
</div>
