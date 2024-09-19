# Continuous Delivery:
### Overview:
### Continuous Delivery vs. Deployment:
- Delivery: Can be deployed to production at any time.
- Deployment: Is automatically deployed to production all the time.
### Build pipeline: automated, Release pipeline: on demand
- Release on demand: control version of software
    - Train users
    - Marketing
    - Timing in general
### Principles:
- Software can be released to production at any time.
- CI is a prerequisite
- DevOps = Developers and Operations working closely together
    - Traditionally incentivized to pursue opposite agendas
- Treat IaC as a code artifact (source control, etc.)
- Automate environment creation and release processes:
    - More automation = 
        - More consistent environment
        - Less human errors
        - Better maintainability
- Again, automated acceptance testing
- Definition of done = running in prod
- Everyone has access to latest result
### Benefits:
- Release takes less effort
    - More automation
- More reliable and repeatable
    - Thanks automation
- Release is more controlled process
- Release more often
- Shorted feedback loops
### Advanced: 
- Blue-green deployment:
    - Two prod envs, one is live
    - Deploy to offline env and test
    - Test and make live
    - Roll back if you have problems
- Canary release:
    - One env
    - Deploy new code to one env, route % to new env
    - Organic acceptance testing
- Feature flags:
    - One env
    - Code is shipped to both
    - Code has parameter to enable/disable feature
    - Combo with Canary, feature enables on % of env
- GitOps:
    - Popular in world of K8s
    - Devs check code into repository
    - Pipeline builds and test, resulting in container
    - Pushed to registry
    - Ops checks into repository
    - Operator process monitors repository
    - Uses changes to modify and create infrastructure
    - Pulls containers from dev container registry.
## Implementation:
1. Have Continuous Integration
2. Unite Developers and Operations
    - Combine teams, DevOps is born
3. Create Release Pipeline
    - Create deployment server
    - Create release definitions
    - Run tests on deployed code
    - Create an IaC Process
        - Script your environment
        - Create release definitions
        - Run tests
        - Make it fast