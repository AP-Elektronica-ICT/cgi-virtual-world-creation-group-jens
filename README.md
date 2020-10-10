# cgi-virtual-world-creation-group-jens

<details>
   <summary>Configuratie Oculus met Unity</summary> 
<br>
   
1. Unity opstarten en een 3D project aanmaken.

<img src="https://user-images.githubusercontent.com/55400627/95658054-49c99380-0b18-11eb-9e9d-63491db6bb1a.png" width="600" />

<img src="https://user-images.githubusercontent.com/55400627/95658099-65349e80-0b18-11eb-8930-d45368fb7d79.png" width="600" />

2. Open Package Manager.

<img src="https://user-images.githubusercontent.com/55400627/95585662-cdfc1800-0a3f-11eb-9559-c500a7614af4.png" width="600" />

3. Installeer de volgende packages. Indien je ze niet ziet, klik op "Advanced" --> "Show preview packages"
    * XR Plugin Management
    * XR Interaction Toolkit (preview)
    * Oculus XR Plugin

<img src="https://user-images.githubusercontent.com/55400627/95586167-9477dc80-0a40-11eb-84c7-19cb42d5d340.png" width="600" />

4. Open Build Settings.

<img src="https://user-images.githubusercontent.com/55400627/95587436-57144e80-0a42-11eb-9c1d-ef49d445ad5f.png" width="600" />

5. Kies "Android" bij platform en voeg de scenes toe. Daarna switch je van platform. Indien je niet kan switchen naar android, moet je de "Android Build Support" module toevoegen
aan je unity project. 

<img src="https://user-images.githubusercontent.com/55400627/95588243-7a8bc900-0a43-11eb-9e5f-fdf454e94958.png" width="600" />

Indien je de module nog moet toevoegen, zie onderstaande screenshots. Restart unity na de installatie.

<img src="https://user-images.githubusercontent.com/55400627/95588383-a444f000-0a43-11eb-978b-03f1eb2ea961.png" width="600" />

<img src="https://user-images.githubusercontent.com/55400627/95588401-aad36780-0a43-11eb-8e7a-38193e7cc78a.png" width="600" />

6. Ga naar "Player Settings" en daarna naar "Oculus".

<img src="https://user-images.githubusercontent.com/55400627/95588894-495fc880-0a44-11eb-991a-f978deb6e152.png" width="600" />

Zorg dat deze vinkjes aanstaan.

<img src="https://user-images.githubusercontent.com/55400627/95589156-a8bdd880-0a44-11eb-9658-a3f36c5116b1.png" width="600" />

7. Klik hierna op "XR Plug-in Management" en zorg ervoor dat "Oculus" aangevinkt staat bij de "Plug-in Providers".

<img src="https://user-images.githubusercontent.com/55400627/95589722-6cd74300-0a45-11eb-9c61-418f40ab666b.png" width="600" />

8. Nu is de Oculus geconfigureerd en kan je beginnen met ontwikkelen
</details>

<details>
<summary>Rondkijken in een virtuele wereld</summary>
<br>
[RECOMMENDED] Installeer de "POLYGON - Starter Pack". Deze is gratis uit de asset store te halen.

<img src="https://user-images.githubusercontent.com/55400627/95658210-015ea580-0b19-11eb-96b2-84dc630be985.png" width="600" />


1. Voeg bij de scene een "Stationary XR Rig" toe.

<img src="https://user-images.githubusercontent.com/55400627/95658720-d2e2c980-0b1c-11eb-9cbd-0c9e1a090e5d.png" width="600" />

2. Bij de XR Rig gaan we nu de "Locomotion System" component toevoegen en daarna de "XR Rig" object toewijzen aan het component.

<img src="https://user-images.githubusercontent.com/55400627/95658762-1b01ec00-0b1d-11eb-8052-77f4fbe99713.png" width="600" />

<img src="https://user-images.githubusercontent.com/55400627/95658813-8c419f00-0b1d-11eb-8b63-37ac869f75ad.png" width="600" />

3. Voeg ook de "Teleportation Provider" component toe bij de XR Rig object en zorg ervoor dat de "Locomotion System" bij de "System" van de "Teleportation Provider" staat.

<img src="https://user-images.githubusercontent.com/55400627/95659796-cada5800-0b23-11eb-9598-732d8bb32743.png" width="600" />

<img src="https://user-images.githubusercontent.com/55400627/95659812-ef363480-0b23-11eb-8dd0-95f8bc33756b.png" width="600" />

4. We hebben ook nog de "Snap Turn Provider" component nodig. Drag daarna de "Locomotion System" naar de "System" van de "Snap Turn Provider".

<img src="https://user-images.githubusercontent.com/55400627/95659915-af238180-0b24-11eb-844b-c826501a6bcc.png" width="600" />

<img src="https://user-images.githubusercontent.com/55400627/95659947-dda15c80-0b24-11eb-850e-eef0fc52d3af.png" width="600" />

5. Bij de "Snap Turn Provider" ga je naar "Controllers" en de "Size" verander je naar "1" zoals op de foto. Dan krijg je een optie bij de "Element 0". Je kan hier de linker of recht controller in plaatsen, afhankelijk van de welke je wilt gebruiken. Zo kan je direct een hoeveelheid graden draaien, afhankelijk van de "Turn Amount" dat je bij "Snap Turn Provider" hebt staan.

<img src="https://user-images.githubusercontent.com/55400627/95660066-b1d2a680-0b25-11eb-8712-7e458960935d.png" width="600" />

6. Nu gebruik je prefabs van de polygon starter packet om een omgeving te maken waarin je wilt rondkijken. De foto hieronder is een voorbeeld.

<img src="https://user-images.githubusercontent.com/55400627/95660254-e2671000-0b26-11eb-91b9-7ae7eeb2386d.png" width="600" />

7. Voordat je gaat builden kan het zijn dat je de "Graphics APIs" moet veranderen. Indien je daar "Vulkan" hebt, moet je "OpenGLES3" boven de "Vulkan" plaatsen.

<img src="https://user-images.githubusercontent.com/55400627/95660361-95376e00-0b27-11eb-98a9-fd3a2acfb259.png" width="600" />

8. Nu kan je builden en het op de Oculus Quest runnen.

<img src="https://user-images.githubusercontent.com/55400627/95660379-ada78880-0b27-11eb-90d4-2b3a50464711.png" width="600" />













