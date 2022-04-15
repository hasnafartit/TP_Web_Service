# TP_Web_Service

Dans cette partie on a creer un web service.

Tout d'abord on a cree la classe Compte 
pui ona cree la classe du web servive 'BanqueService' où on a ajouter les annotations  '@WebService' pour definir le web service, '@'@WebMethod' pour definir les methodes et '@WebParam' pour definir les paramatere 

![image](https://user-images.githubusercontent.com/84719124/163244495-1d17c1ab-651b-4861-856e-01a347cdc5b4.png)

si on ecrit sur le navigateur le url suivant " http://localhost:8686/BanqueWS?wsdl " il donne le WSDL


![image](https://user-images.githubusercontent.com/84719124/163244560-90ced091-49b8-48cc-9ce5-a39e732f9ac2.png)

 http://localhost:8686/?xsd=1
 
![image](https://user-images.githubusercontent.com/84719124/163244598-6ef2bc59-fdf7-424b-ab62-aef6b33a795c.png)


miantenant on va tester le web service
on a testé les methodes du web service en utilisant SoapUI


![image](https://user-images.githubusercontent.com/84719124/163244667-e676ab2d-a356-43d2-b243-5af21bb15ca6.png)


tester getcompte


![image](https://user-images.githubusercontent.com/84719124/163244725-c7e7fc30-0354-40c9-97e1-9f01929a0a66.png)


test listCompte

![image](https://user-images.githubusercontent.com/84719124/163244872-3baa4d7b-3d00-4b5f-a1fe-565493a60327.png)


JaxB
on a utilisé l'annotation @XmlRootElement pour convertir un Objet en XML
l'annotation @XmlTransient est utilisé par defaut pour les getters et les setters et on a utilisé l'annotation @XmlAccessorType(XmlAccessType.FIELD) pour que l'annotation @XmlTransient soit utilisé directement sur les attributs c-à-d pour ignorer des attributs 


![image](https://user-images.githubusercontent.com/84719124/163244944-a8b3ffbf-55d0-41a9-8af8-1eba082ad49e.png)

![image](https://user-images.githubusercontent.com/84719124/163244963-e9706d10-a226-488a-b5e7-0538caecc336.png)



Apres on a creé un client java
jaxWS joue le role de SKELETON
ET ON A generer un proxy(joue le role de STUP) à  partir du wsdl puis on a creer la classe ClientWS ou on a creer la classe main 


![image](https://user-images.githubusercontent.com/84719124/163245023-5b5a87be-d75d-4380-99ca-06e41a699bde.png)



![image](https://user-images.githubusercontent.com/84719124/163245054-4cc6080f-9350-4535-9af3-53220abe12fd.png)



on peut aussi generer le code sur le terminal par la commande  wsimport -s . http://localhost:8686/BanqueWS?wsdl



![image](https://user-images.githubusercontent.com/84719124/163245111-32e0283f-199a-4fab-b74f-674a6502122c.png)


![image](https://user-images.githubusercontent.com/84719124/163245147-e1a6ac48-25b6-4e00-87ba-56783fa66203.png)

![image](https://user-images.githubusercontent.com/84719124/163245525-a690bee1-bdf5-4bb8-b3ba-e817f5c8031e.png)


![image](https://user-images.githubusercontent.com/84719124/163245178-c439fc3a-8551-4bf0-ab77-a1e31ca80cfa.png)




