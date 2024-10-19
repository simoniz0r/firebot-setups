# Setup

- Import `Break_Clip_Loop.firebotsetup` by clicking `File` -> `Import Firebot Setup...` and then browse to the location you downloaded the above file.

- Enable Firebot Overlay Instances by going to `Settings` -> `Overlay` and toggling `Overlay Instances` to `On`.

- While still in the Overlay settings, click `Edit Instances`, then click `Create Instance`, enter `Breaks` as the name, click `Create`, and then `Done`.

- If you have not already done so, connect OBS to Firebot under `Settings` -> `Integrations`.

- Go to `Events` -> `OBS` and edit both the `start break clip loop` and `stop break clip loop` effects so that the `Scene Name` under `Filters` matches the name of your break scene in OBS as shown in the screenshot below:

![img](https://dl.imgix.net/clip_loop_scene.png)

- If you would like to change the time frame the clip loop fetches clips for, go to `Events` -> `OBS` and edit the `start break clip loop`.  Click the `Run Effect List` effect, and then change the `Days` preset argument to the max amount of days to fetch clips for as shown in the screenshot below:

![img](https://dl.imgix.net/clip_loop_time.png)

- In OBS, add a new browser source configured as shown in the screenshot below: 

![img](https://dl.imgix.net/clip_loop_obs.png)

- In Firebot, go to `Events` -> `OBS` and enable all 3 of the events included with this setup.

- If you have setup everything correctly, the clip loop will start any time you switch to your break scene in OBS, and it will stop when you switch from the break scene to any other scene.
