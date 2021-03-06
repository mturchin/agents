<div itemscope itemtype="http://developers.google.com/ReferenceObject">
<meta itemprop="name" content="tf_agents.trajectories.time_step.TimeStep" />
<meta itemprop="path" content="Stable" />
<meta itemprop="property" content="step_type"/>
<meta itemprop="property" content="reward"/>
<meta itemprop="property" content="discount"/>
<meta itemprop="property" content="observation"/>
<meta itemprop="property" content="is_first"/>
<meta itemprop="property" content="is_last"/>
<meta itemprop="property" content="is_mid"/>
</div>

# tf_agents.trajectories.time_step.TimeStep

<table class="tfo-notebook-buttons tfo-api" align="left">
</table>

<a target="_blank" href="https://github.com/tensorflow/agents/tree/master/tf_agents/trajectories/time_step.py">View
source</a>

## Class `TimeStep`

Returned with every call to `step` and `reset` on an environment.



<!-- Placeholder for "Used in" -->

A `TimeStep` contains the data emitted by an environment at each step of
interaction. A `TimeStep` holds a `step_type`, an `observation` (typically a
NumPy array or a dict or list of arrays), and an associated `reward` and
`discount`.

The first `TimeStep` in a sequence will equal
<a href="../../../tf_agents/trajectories/time_step/StepType.md#FIRST"><code>StepType.FIRST</code></a>.
The final `TimeStep` will equal
<a href="../../../tf_agents/trajectories/time_step/StepType.md#LAST"><code>StepType.LAST</code></a>.
All other `TimeStep`s in a sequence will equal `StepType.MID.

#### Attributes:

* <b>`step_type`</b>: a `Tensor` or array of `StepType` enum values.
* <b>`reward`</b>: a `Tensor` or array of reward values.
* <b>`discount`</b>: A discount value in the range `[0, 1]`.
* <b>`observation`</b>: A NumPy array, or a nested dict, list or tuple of arrays.

## Properties

<h3 id="step_type"><code>step_type</code></h3>

<h3 id="reward"><code>reward</code></h3>

<h3 id="discount"><code>discount</code></h3>

<h3 id="observation"><code>observation</code></h3>

## Methods

<h3 id="is_first"><code>is_first</code></h3>

<a target="_blank" href="https://github.com/tensorflow/agents/tree/master/tf_agents/trajectories/time_step.py">View
source</a>

``` python
is_first()
```

<h3 id="is_last"><code>is_last</code></h3>

<a target="_blank" href="https://github.com/tensorflow/agents/tree/master/tf_agents/trajectories/time_step.py">View
source</a>

``` python
is_last()
```

<h3 id="is_mid"><code>is_mid</code></h3>

<a target="_blank" href="https://github.com/tensorflow/agents/tree/master/tf_agents/trajectories/time_step.py">View
source</a>

``` python
is_mid()
```
