+++
type = "rivanna"
categories = [
  "HPC",
  "software",
]
date = "2023-09-08T00:00:00-05:00"
tags = [
  "lang",
]
draft = false
shorttitle = "Code Server"
modulename = "code-server"
softwarename = "Code Server"
title = "Code Server on Rivanna"
author = "RC Staff"

+++

# Description
{{< module-description >}}

**Software Category:** {{% module-category %}}

For detailed information, visit the [{{% software-name %}} website]({{< module-homepage >}}).

# Available Versions
To find the available versions and learn how to load them, run:
```
module spider {{% module-name %}}
```

The output of the command shows the available {{% software-name %}} module versions.

For detailed information about a particular {{% software-name %}} module, including how to load the module, run the `module spider` command with the module's full version label. __For example__:
```
module spider {{% module-firstversion %}}
```

{{< module-versions >}}

# Interactive Sessions through Rivanna's Web Portal

Interactive sessions of {{% software-name %}} can be launched through Rivanna's web portal, [Open OnDemand](/userinfo/rivanna/ood/overview).
If you are new to Rivanna, you may want to read the [Getting Started Guide](/userinfo/rivanna/queues/) to learn more about the partitions.

## Python Setup

Python users should install the `ms-python` extension and select an appropriate interpreter, unless you wish to use the system python (2.7):

1. Press F1
1. Search for “python: select interpreter”
1. Choose the anaconda python or any other python in your custom environments.

## Closing the Interactive Session
When you are done, delete the {{% software-name %}} session from the "My Interactive Sessions" tab and the allocated resources will be released.
