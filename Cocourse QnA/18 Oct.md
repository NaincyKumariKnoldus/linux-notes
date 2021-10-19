### What is the difference between Build and Task?
   The smallest configurable unit in a Concourse pipeline is a single task. A task can be thought of as a function from task.inputs to task.outputs that can either succeed or fail.Whereas A build is an execution of a build plan.
   
### Difference between resource and Resource type?
   Resource :A resource in concource is some sort of entity that stores data. Things that are happening on the server typically a lot of stuff is not saved. Resource are how concource interacts with the outside world.The main goal of resource is to represent some external system or object in your pipeline.

Resource Types :Each resource in a pipeline has a type. The resource's type determines what versions are detected, the bits that are fetched when the resource's get step runs, and the side effect that occurs when the resource's put step runs. Concourse comes with a few "core" resource types to cover common use cases like git and s3 - the rest are developed and supported by the Concourse community.

### What is a webnode?
  The web node is responsible for running the web UI, API, and as well as performing all pipeline scheduling. It's basically the brain of Concourse.
  
### What is a worker node?
  The worker node registers with the web node and is then used for executing builds and performing resource checks. It doesn't really decide much on its own.
  
### How do ATC & TSA communicate?
   The TSA starts heartbeating every 30 seconds, pinging the worker for its current number of Garden containers and Baggageclaim volumes, and sending updated information to the ATC. If the worker fails to respond, the TSA notifies ATC that worker is stalled.This Atc and Tsa Communicate via API.

### Where does the worker node run in our system?
  The worker node registers with the web node and is then used for executing builds and performing resource checks. It doesn't really decide much on its own. CONCOURSE_WORK_DIR=/opt/concourse/worker
### Difference between error and failed?
  Error : Refers to difference between Actual Output and Expected output.\
  Failure : It is the inability of a system or component to perform required function according to its specification.
  
### Can other team see the build logs after expose-pipeline?
  Every newly configured pipeline is hidden to anyone but the pipeline's team. To make a pipeline publicly viewable, both by other teams and unauthenticated users, see fly expose-pipeline.

  Even with a pipeline exposed, all build logs are hidden by default. This is because CI jobs are prone to leaking credentials and other...unsavory information. After you've determined that a job's builds should be safe for public consumption, you can set public: true on the job in your pipeline.
