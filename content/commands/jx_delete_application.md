---
date: 2018-12-14T12:42:41Z
title: "jx delete application"
slug: jx_delete_application
url: /commands/jx_delete_application/
---
## jx delete application

Deletes one or more applications from Jenkins

### Synopsis

Deletes one or more Applications 

Note that this command does not remove the underlying Git Repositories. 

For that see the https://jenkins-x.io/commands/jx_delete_repo/command.

```
jx delete application [flags]
```

### Examples

```
  # prompt for the available apps to delete
  jx delete app
  
  # delete a specific app
  jx delete app cheese
```

### Options

```
  -a, --all                             Selects all the matched applications
  -b, --batch-mode                      Run without being prompted. WARNING! You will not be asked to confirm deletions if you use this flag.
  -f, --filter string                   Filter the list of applications to those containing this text
  -h, --help                            help for application
      --no-env                          Do not remove the application from any of the Environments
      --no-merge                        Disables automatic merge of promote Pull Requests
  -o, --org string                      github organisation/project name that source code resides in. Temporary workaround until the platform can determine this automatically
      --pull-request-poll-time string   Poll time when waiting for a Pull Request to merge (default "20s")
  -t, --timeout string                  The timeout to wait for the promotion to succeed in the underlying Environment. The command fails if the timeout is exceeded or the promotion does not complete (default "1h")
```

### SEE ALSO

* [jx delete](/commands/jx_delete/)	 - Deletes one or more resources

###### Auto generated by spf13/cobra on 14-Dec-2018
