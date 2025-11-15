# microphone
## mic sounds like you come from Cybertron?
1. "Mic Boost" too high
    * Using alsa-utils to lower your mic boost
    * NEVER set auto-volume-for-microphone in wemeet
2. unproperate back rate
    * lower the rate in config to pipewire
## too noisy
1. use a noice-reduction program
    * noise-suppression-for-voice
    ```bash
    pacman -S noise-suppression-for-voice
    ```
    > following guidance in <https://github.com/werman/noise-suppression-for-voice>
# speaker
## no sound comming out of speaker
1. check daemon service
    ```bash
    systemctl status --user pipewire.service
    ```
2. if not run properly
    * check log file for systemd
3. it's running properly
    * check audio device
        * using "alsa-utils"
            * if audio device exists : maximise speaker volume in "alsa-utils"
            * if not : hardware error
 