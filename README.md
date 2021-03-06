# MADDPG in Ray/RLlib

## Please tell me if you have problems with this code
MADDPG is not in a 100% bug free state, and hence is in /contrib in rllib. Getting MADDPG fully working is important to me. If you have a problem, please let me know.

## Notes
-This was forked from wsjeons's original repo due to lack of maintenance
- The codes in [OpenAI/MADDPG](https://github.com/openai/maddpg) were refactored in RLlib, and test results are given in `./plots`.
    - It was tested on 7 scenarios of [OpenAI/Multi-Agent Particle Environment (MPE)](https://github.com/openai/multiagent-particle-envs).
        - `simple`, `simple_adversary`, `simple_crypto`, `simple_push`, `simple_speaker_listener`, `simple_spread`, `simple_tag`
            - RLlib MADDPG shows the similar performance as OpenAI MADDPG on 7 scenarios except `simple_crypto`. 
    - Hyperparameters were set to follow the original hyperparameter setting in [OpenAI/MADDPG](https://github.com/openai/maddpg).
    
- Empirically, *removing lz4* makes running much faster. I guess this is due to the small-size observation in MPE. 
    

## References
- [OpenAI/MADDPG](https://github.com/openai/maddpg)
- [OpenAI/Multi-Agent Particle Environment](https://github.com/openai/multiagent-particle-envs)
    - [wsjeon/Multi-Agent Particle Environment](https://github.com/wsjeon/multiagent-particle-envs)
        - It includes the minor change for MPE to work with recent OpenAI Gym.

 
