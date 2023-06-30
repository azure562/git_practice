---
title: "Use Github Repo Secret in Python (without Action)"
description: ""
date: 2023-06-30T18:17:35Z
keywords: []
---

If you google "how to use github secrets and variables in python", almost all the answers talk about GitHub Actions/workflows.

But, does it have to be so?

ChatGPT just showed me, "No!"

> When you add the XXX API access key as a repository secret in GitHub, you can access it within your Python script by using the os module to access environment variables. Here's how you can refer to the access key in your script:

```python
import os

access_key = os.environ.get('YOUR_PET_API_ACCESS_KEY')

# Check if the access key is available
if access_key is None:
    print("PET API access key not found. Please set the 'YOUR_PET_API_ACCESS_KEY' environment variable.")
    exit()
```
