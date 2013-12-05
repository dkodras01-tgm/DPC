--Server starten

start rmiregistry

java -cp c:\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src\;c:\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src\compute.jar -Djava.rmi.server.codebase=file:\c:\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src\compute.jar -Djava.rmi.server.hostname=localhost -Djava.security.policy=server.policy engine.ComputeEngine


--Client starten (in neuen cmd)

java -cp c:\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src;c\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src\compute.jar -Djava.rmi.server.codebase=file:\c:\Users\Acer\Desktop\Schule\4AHIT\SEW\Programme\DPC\src -Djava.security.policy=client.policy client.ComputePi localhost 45