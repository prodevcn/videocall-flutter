import 'dart:io';
String strCert = ("""
-----BEGIN CERTIFICATE-----
MIIDBjCCAe4CCQCuf5QfyX2oDDANBgkqhkiG9w0BAQsFADBFMQswCQYDVQQGEwJB
VTETMBEGA1UECAwKU29tZS1TdGF0ZTEhMB8GA1UECgwYSW50ZXJuZXQgV2lkZ2l0
cyBQdHkgTHRkMB4XDTE0MDkyOTA5NDczNVoXDTE1MDkyOTA5NDczNVowRTELMAkG
A1UEBhMCQVUxEzARBgNVBAgMClNvbWUtU3RhdGUxITAfBgNVBAoMGEludGVybmV0
IFdpZGdpdHMgUHR5IEx0ZDCCASIwDQYJKoZIhvcNAQEBBQADggEPADCCAQoCggEB
AMJOyOHJ+rJWJEQ7P7kKoWa31ff7hKNZxF6sYE5lFi3pBYWIY6kTN/iUaxJLROFo
FhoC/M/STY76rIryix474v/6cRoG8N+GQBEn4IAP1UitWzVO6pVvBaIt5IKlhhfm
YA1IMweCd03vLcaHTddNmFDBTks7QDwfenTaR5VjKYc3OtEhcG8dgLAnOjbbk2Hr
8wter2IeNgkhya3zyoXnTLT8m8IMg2mQaJs62Xlo9gs56urvVDWG4rhdGybj1uwU
ZiDYyP4CFCUHS6UVt12vADP8vjbwmss2ScGsIf0NjaU+MpSdEbB82z4b2NiN8Wq+
rFA/JbvyeoWWHMoa7wkVs1MCAwEAATANBgkqhkiG9w0BAQsFAAOCAQEAYLRwV9fo
AOhJfeK199Tv6oXoNSSSe10pVLnYxPcczCVQ4b9SomKFJFbmwtPVGi6w3m+8mV7F
9I2WKyeBHzmzfW2utZNupVybxgzEjuFLOVytSPdsB+DcJomOi8W/Cf2Vk8Wykb/t
Ctr1gfOcI8rwEGKxm279spBs0u1snzoLyoimbMbiXbC82j1IiN3Jus08U07m/j7N
hRBCpeHjUHT3CRpvYyTRnt+AyBd8BiyJB7nWmcNI1DksXPfehd62MAFS9e1ZE+dH
Aavg/U8VpS7pcCQcPJvIJ2hehrt8L6kUk3YUYqZ0OeRZK27f2R5+wFlDF33esm3N
dCSsLJlXyqAQFg==
-----END CERTIFICATE-----
""");
String strKey = ("""
-----BEGIN RSA PRIVATE KEY-----
MIIEogIBAAKCAQEAwk7I4cn6slYkRDs/uQqhZrfV9/uEo1nEXqxgTmUWLekFhYhj
qRM3+JRrEktE4WgWGgL8z9JNjvqsivKLHjvi//pxGgbw34ZAESfggA/VSK1bNU7q
lW8Foi3kgqWGF+ZgDUgzB4J3Te8txodN102YUMFOSztAPB96dNpHlWMphzc60SFw
bx2AsCc6NtuTYevzC16vYh42CSHJrfPKhedMtPybwgyDaZBomzrZeWj2Cznq6u9U
NYbiuF0bJuPW7BRmINjI/gIUJQdLpRW3Xa8AM/y+NvCayzZJwawh/Q2NpT4ylJ0R
sHzbPhvY2I3xar6sUD8lu/J6hZYcyhrvCRWzUwIDAQABAoIBACwt56TW3MZxqZtN
8WYsUZheUispJ/ZQMcLo5JjOiSV1Jwk+gpJtyTse291z+bxagzP02/CQu4u32UVa
cmE0cp+LHO4zB8964dREwdm8P91fdS6Au/uwG5LNZniCFCQZAFvkv52Ef4XbzQen
uf4rKWerHBck6K0C5z/sZXxE6KtScE2ZLUmkhO0nkHM6MA6gFk2OMnB+oDTOWWPt
1mlreQlzuMYG/D4axviRYrOSYCE5Qu1SOw/DEOLQqqeBjQrKtAyOlFHZsIR6lBfe
KHMChPUcYIwaowt2DcqH/A+AFXRtaifa6DvH8Yul+2vAp47UEpaenVfM5bpN33XV
EzerjtECgYEA+xiXzblek67iQgRpc9eHSoqs4iRLhae8s8kpAG51Jz46Je+Dmium
XV769oiUGUxBeoUb7ryW+4MOzHJaA1BfGejQSvwLIB9e4cnikqnAArcqbcAcOCL1
aYYDiSmSmN/AokNZlPKEBFXP9bzXrU9smQJWNTHlcRl7JXfnwF+jwNsCgYEAxhpE
SBr9vlUVHNh/S6C5i80NIYg6jCy2FgsmuzEqmcqV0pTyzegmq8bru+QmuvoUj2o4
nVv4J9d1fLF6ECUVk9aK8UdJOOB6hAfurOdJCArgrsY/9t4uDzXfbPCdfSNQITE0
XgeNGQX1EzvwwkBmyZKk0kLIr3syP8ZCWfXDROkCgYBR+dF1pJMv++R6UR5sZ20P
9P5ERj0xwXVl7MKqFWXCDhrFz9BTQPTrftrIKgbPy4mFCnf4FTHlov/t11dzxYWG
2+9Ey8yGDDfZ1yNVZn39ZPdBJXsRCLi+XrZAzYXCyyoEz6ArdJGNKMbgH2r6dfeq
bIzgiQ2zQvJlZSQQNiksCQKBgCgwzAmU8EXdHRttEOZXBU3HnBJhgP9PUuHGAWWY
4/uvjhXbAiekIbRX9xt3fiQQ+HrgIfxK3F246K0TlKAR5f7IWAf7Xm+bmz+OHG4X
vklTa6IJtpBvIwkS9PE1H75zm54gTW+GOKoK+12bm4zNZA0hIy9FPVHcvKUTpAJ8
SdGBAoGAHLtJnB1NO4EgO6WtLQMXt7HrIbup8eZi8/82gC3422C+ooKIrYQ07qSw
nBOO/G0OB4yd6vCE2x5+TWSSCYGgG5A8aIv5qP76RP4hovGHxG/y2tfotw5UuOrh
nFWlTP4Urs8PeykvK9ao8r/T8BnPIC16U6ENYvAc0mRlFA2j1GA=
-----END RSA PRIVATE KEY-----
""");

class Server {
  var clients = new Set();
  var _socket;
  var sessions = [];
  
  Future<void> init() async {
    // SecurityContext context = new SecurityContext({true});
    
    // var chain =
    //    Platform.script.resolve('cert.pem')
    //    .toFilePath();
    // var key =
    //    Platform.script.resolve('key.pem')
    //    .toFilePath();
    // context.useCertificateChain(chain);
    // context.usePrivateKey(key);
    

    HttpServer.bindSecure(InternetAddress.anyIPv4, 4443, SecurityContext.defaultContext)
        .then((server) {
          print("Secure server listening on 4443...");
          //server.serverHeader = "Secure WebSocket server";
          server.listen((HttpRequest request) {
            print(" receive request .....................");
            if (request.headers.value(HttpHeaders.UPGRADE) == "websocket"){
              WebSocketTransformer.upgrade(request).then(handleWebSocket);
              print(" upgrade websocket .....................");
            }
            else {
              request.response.statusCode = HttpStatus.FORBIDDEN;
              request.response.reasonPhrase = "WebSocket connections only";
              request.response.close();
              print(" websocket connections only.....................");
            }
          });
        });
  }
  Future<void> updatePeers () async {
    var peers = [];
    this.clients.forEach((client) {
            var peer = {};
            if (client.hasOwnProperty('id')) {
              peer['id'] = client.id;
            }
            if (client.hasOwnProperty('name')) {
                peer['name'] = client.name;
            }
            if (client.hasOwnProperty('user_agent')) {
                peer['user_agent'] = client.user_agent;
            }
            if (client.hasOwnProperty('session_id')) {
                peer['session_id'] = client.session_id;
            }
            peers.add(peer);
        });
        var msg = {
            "type": "peers",
            "data": peers,
        };
        this.clients.forEach((client) {
          _send(msg.toString());
        });
  }

  void onClose(clientSelf) {
    print('client is close');
    var sessionId = clientSelf['session_id'];
    //remove old session_id
    if (sessionId) {
            for (var i = 0; i < this.sessions.length; i++) {
                var item = this.sessions[i];
                if (item.id == sessionId) {
                    this.sessions.removeAt(i);
                    break;
                }
            }
        }
        var msg = {
            'type': "leave",
            'data': clientSelf.id,
        };

        this.clients.forEach((client) {
            if (client != clientSelf)
            _send(msg.toString());
        });

        this.updatePeers();
  }

  void handleWebSocket(WebSocket socket){
    _socket = socket;
      print("Secure client connected! ===============================");
    socket.listen((data) {
      print("Secure client connected!");
      this.clients.add(_socket);

       this.onMessage(data);
    },
    onDone: () {
      print('Client disconnected');
      this.clients.remove(_socket);
      this.onClose(_socket);
    });
  }

  void onMessage(message) async {
    Map<String, dynamic> mapData = message;
    var data = mapData['data'];
    print("message.type : " + mapData['type'] + ", \nbody: " + data.toString());

    switch (mapData['type']) {
      case 'new':
      {
        //_socket['id'] = data.id;

      }
      break;
      case 'bye':
      {

      }
      break;
      case 'offer':
      {

      }
      break;
      case 'answer':
      {

      }
      break;
      case 'candidate':
      {

      }
      break;
      case 'keepalive':
      {

      }
      break;
      default:
        break;
    }
  }

  void _send(message) {
    try {
      if (_socket != null) {
      _socket.add(message);
      print('send data success , data is : $message');
    }
    } catch (e) {
      print("send failure !: " + e);
    }
  }

}
