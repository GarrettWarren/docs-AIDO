# Your first submission {#cm-first status=ready}

This section describes the steps to make your first submission.

## Checkout the submission repo {#cm-first-checkout}

Check out the submission template [`challenge-aido1_luck-template-python`][template]:

    $ git clone -b v4 https://github.com/duckietown/challenge-aido1_luck-template-python.git
    

[template]: https://github.com/duckietown/challenge-aido1_luck-template-python


## Submit {#cm-first-submit}

Go to the repository root:

    $ cd challenge-aido1_luck-template-python

Submit using:

    $ dts challenges submit
    
What this does is:

1. Build a Docker container.
2. Push the Docker container.
3. Make contact with the [challenge server][server] to send your submission.

[server]: https://challenges.duckietown.org/v4/

The expected output is something along the lines of:

    Sending build context to Docker daemon  5.632kB
    ...
    ...
    Successfully created submission 23
    
    You can track the progress at: https://challenges.duckietown.org/v4/humans/submissions/23
    
    You can also use the command:
    
       dts challenges follow --submission 23

## Monitor the submission {#cm-first-monitor}

There are 2 ways to monitor the submission:

The first way is to use the web interface, at the URL indicated; in the example, this is:


> [`https://challenges.duckietown.org/v4/humans/submissions/2`](https://challenges.duckietown.org/v4/humans/submissions/2)

The second way is to use the `dts challenges follow` command:

     $ dts challenges follow --submission ![submission ID]
     
     
## Look at the leaderboard {#cm-first-leaderboard}


The leaderboard is available at the URL 

> [`https://challenges.duckietown.org/v4/humans/challenges/aido4_luck-v4/leaderboard`][leaderboard]
    
    
[leaderboard]: https://challenges.duckietown.org/v4/humans/challenges/aido2_luck-v4/leaderboard


      
     
## Local evaluation {#cm-local}

You can also evaluate the submission *locally*.  This is useful for debugging and development.

Use this command:

    $ dts challenges evaluate 
    
### Troubleshooting

If any of the commands above don't work, it is likely that something
related to Docker permissions is to blame - please file an issue, as we are trying to fix that problem.

