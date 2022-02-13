# casparcg-connect (subflow)
Node-Red Subflow to build up an amcp and osc connection to a casparcg server

## casparcg
- downloads: https://github.com/CasparCG/Server/releases?after=v2.3.3-lts-stable
- documentation: https://github.com/CasparCG/help/wiki
- testet version: 2.3.3-lts-stable

### casparcg.config
be shure to have these tags included:

```
  <controllers>
    <tcp>
      <port>5250</port>
      <protocol>AMCP</protocol>
    </tcp>
  </controllers>
  <amcp>
    <media-server>
      <host>localhost</host>
      <port>8000</port>
    </media-server>
  </amcp>
  <osc>
    <default-port>6250</default-port>
    <disable-send-to-amcp-clients>false</disable-send-to-amcp-clients>
    <predefined-clients>
      <predefined-client>
        <address>127.0.0.1</address>
        <port>5253</port>
      </predefined-client>
    </predefined-clients>
  </osc>
```


## flow
![image](https://user-images.githubusercontent.com/4168388/153772933-b232418b-8305-478f-9e39-b146e470f755.png)

## subflow
![image](https://user-images.githubusercontent.com/4168388/153772999-fec8fd1c-5662-4f2f-a92f-dce275ea26fb.png)
### connection settings
- udp: <br>![image](https://user-images.githubusercontent.com/4168388/153750762-33782994-3db1-4da1-9d11-b6277a03d769.png)
- tcp: <br>![image](https://user-images.githubusercontent.com/4168388/153750842-bfa788cb-68e0-47af-a670-939503618fb6.png) 
