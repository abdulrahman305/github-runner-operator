<!-- markdownlint-disable -->

<a href="../src/github_client.py#L0"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

# <kbd>module</kbd> `github_client.py`
GitHub API client. 

Migrate to PyGithub in the future. PyGithub is still lacking some API such as remove token for runner. 



---

## <kbd>class</kbd> `GithubClient`
GitHub API client. 

<a href="../src/github_client.py#L25"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `__init__`

```python
__init__(token: str, request_session: Session)
```

Instantiate the GiHub API client. 



**Args:**
 
 - <b>`token`</b>:  GitHub personal token for API requests. 
 - <b>`request_session`</b>:  Requests session for HTTP requests. 




---

<a href="../src/github_client.py#L142"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `delete_runner`

```python
delete_runner(path: Union[GithubOrg, GithubRepo], runner_id: int) → None
```

Delete the self-hosted runner from GitHub. 



**Args:**
 
 - <b>`path`</b>:  GitHub repository path in the format '<owner>/<repo>', or the GitHub organization  name. 
 - <b>`runner_id`</b>:  Id of the runner. 

---

<a href="../src/github_client.py#L36"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `get_runner_applications`

```python
get_runner_applications(
    path: Union[GithubOrg, GithubRepo]
) → List[RunnerApplication]
```

Get list of runner applications available for download. 



**Args:**
 
 - <b>`path`</b>:  GitHub repository path in the format '<owner>/<repo>', or the GitHub organization  name. 

**Returns:**
 List of runner applications. 

---

<a href="../src/github_client.py#L55"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `get_runner_github_info`

```python
get_runner_github_info(
    path: Union[GithubOrg, GithubRepo]
) → list[SelfHostedRunner]
```

Get runner information on GitHub under a repo or org. 



**Args:**
 
 - <b>`path`</b>:  GitHub repository path in the format '<owner>/<repo>', or the GitHub organization  name. 



**Returns:**
 List of runner information. 

---

<a href="../src/github_client.py#L120"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `get_runner_registration_token`

```python
get_runner_registration_token(path: Union[GithubOrg, GithubRepo]) → str
```

Get token from GitHub used for registering runners. 



**Args:**
 
 - <b>`path`</b>:  GitHub repository path in the format '<owner>/<repo>', or the GitHub organization  name. 



**Returns:**
 The registration token. 

---

<a href="../src/github_client.py#L102"><img align="right" style="float:right;" src="https://img.shields.io/badge/-source-cccccc?style=flat-square"></a>

### <kbd>function</kbd> `get_runner_remove_token`

```python
get_runner_remove_token(path: Union[GithubOrg, GithubRepo]) → str
```

Get token from GitHub used for removing runners. 



**Returns:**
  The removing token. 

