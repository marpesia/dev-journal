# Always test in every deployment environment

## The problem
I migrated a frontend library and updated some routes.
Tested locally with Docker -> everything work
Deployed to the cloud on Kubernetes -> it broke

## What I found out
Local and cloud environments had different app configurations.
The routes that worked in one didn't resolve the same way in the other.

## Why it matters
Passing local test is not enough. If the app has different configurations per environment, each one needs to be tested before calling it done.