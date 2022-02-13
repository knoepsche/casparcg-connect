# casparcg-connect (subflow)
Node-Red Subflow to send amcp to a casparcg server and get osc from a casparcg server<br>

## casparcg
- downloads: https://github.com/CasparCG/Server/releases?after=v2.3.3-lts-stable
- documentation: https://github.com/CasparCG/help/wiki

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
![image](https://user-images.githubusercontent.com/4168388/153750033-a806be78-6aa5-4be1-84a0-d45d8ded78e9.png)

## subflow
![image](https://user-images.githubusercontent.com/4168388/153749967-d6578a94-6c56-457e-8604-efc35245c118.png)
### connection settings
- udp: <br>![image](https://user-images.githubusercontent.com/4168388/153750762-33782994-3db1-4da1-9d11-b6277a03d769.png)
- tcp: <br>![image](https://user-images.githubusercontent.com/4168388/153750842-bfa788cb-68e0-47af-a670-939503618fb6.png) 
