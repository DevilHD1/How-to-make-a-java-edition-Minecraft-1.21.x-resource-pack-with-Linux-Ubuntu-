# How-to-make-a-java-edition-Minecraft-1.21.x-resource-pack-with-Linux-Ubuntu
1. Make a folder and name it however you like.
--------------------------------------------------------------------
2. Make a file and rename it pack.mcmeta .
---------------------------------------------------------------------
3. Paste 

{
  "pack": {
    "pack_format": 65,     <--This is the Minecraft version(variates)
    "description": "This is a testpack"
  }
}
    
into the file in a file editor.
---------------------------------------------------------------------
4. Format the pack in the the terminal by pasting:
   "cd [Path to your resource pack folder]" 
   for example: cd Documents/pack.mcmeta .
   Open the file with nano:
   "nano pack.mcmeta"
   (If nano is not installed, run: "sudo apt install nano")
---------------------------------------------------------------------
5. Save and exit it by pushing:             
   Ctrl+O; Enter; Ctrl+X in the menu
---------------------------------------------------------------------
6. If you want to have a different icon shown in the pack menu in Minecraft you can paste a 128x128 pixel .png picture into your pack folder.
---------------------------------------------------------------------
7. Create subfolder called assets in your resource pack folder.
   The subfolder: assets, the icon: [The name of it].png and the 
   pack.mcmeta file: pack.mcmeta should be the only  
   files located in the main folder directly. All other other   	
   resource files must be located somewhere in assets or they won't 
   be read by Minecraft. 
---------------------------------------------------------------------
8. Inside the assets folder you should make your namespace folders.
   If you are modifying the vanilla resources, they should go into   
   the minecraft namespace folder. If you are making custom 
   additions they should go in your own namespace folder(You should 
   pick a unique namespace name so that it does not get confused with 	
   any other Minecraft resource packs).  
---------------------------------------------------------------------
9. If you plan on editing multiple Minecraft resources or to help  
   ease the access, you should save copies of the vanilla 
   resources in an accessible location in case some things rely on   
   other files within the directory. To do this, you have to 	 
   open the Minecraft launcher, go to installations and hover over 
   the Minecraft installation that you are using. You will see a 
   folder icon the name of the installation, for example: Latests 
   release and a Minecraft icon on the left next to it. You should 
   see a button that says play, three dots and a folder icon on 
   the right. You want to open the .minecraft directory, so left 
   click on the folder icon to do so. It will open up the .minecraft  	
   directory. Here you open the versions folder. There will be a   
   list of numbered folders, which correspond to the versions/ 
   installation you have loaded or have loaded in the past.
---------------------------------------------------------------------
10. Now what you want to do, is open the Minecraft version you     
    want to use for your vanilla resources. It will show you   	   
    [The Minecraft version].json file and the [The Minecraft  
    version].jar file. You must extract the .jar file by   
    right-clicking on the file and clicking: Extract to here. (You 
    may also use a file loader to do so, by clicking on opne with:
    and then your loader or you can simply change the format
    from .jar to .zip) 
---------------------------------------------------------------------
11. In the folder that was created in 10 you should navigate to 
    assets-->minecraft-->textures
    Here you can find your assets for the creation of your  
    resourcepack. For now we are going to use the creeper. So 
    navigate to entity-->creeper, where you can find the 
    creeper.png. Save a duplicate of this somewhere accessible or 
    keep this folder open window open during the next steps. Now you 
    have to replicate the folder structure, so that Minecraft knows 
    to use that texture. So in your assets folder in your main 
    resourcepack folder, you should have a folder called minecraft 
    already. In this folder, you should make a subfolder called 
    textures. In this folder, you should make a subfolder called 
    entity. In this folder, you should make a subfolder called the  
    entity that you are using, in my case, the creeper, so here we 
    make a folder called creeper. Copy the creeper texture from the 
    vanilla resource pack into your newly created creeper folder.  
    Open the .png file with an image editor of your choice by right- 
    clicking it and selecting "Open With".
    (When you are done, do not forget to save it  
    in the same place, in this case in assets->minecraft->textures
    ->entity->creeper. Replace the original creeper.png with yours 
    but it should have the same name, so creeper.png .
---------------------------------------------------------------------
12. If you want to replace a block texture or an item, you have to 
    make a new subfolder called block in assets->minecraft->textures
    in your main resourcepack folder. First you think of a block 
    that you would like to edit. If you are just doing a 
    nonanimated texturepack, you simply have to do it like in the 
    step 11 . You can get your original vanilla minecraft block   
    textures in the .minecraft->versions->[The Minecraft version]
    ->[Your extracted Minecraft .jar file from 10]->assets
    ->minecraft->textures->block . If you want to edit a item 
    texture, you may find it under .minecraft->versions->[The 
    Minecraft version]->[Your extracted Minecraft .jar file from 10]
    ->assets->minecraft->textures->items .
    In case you want to make a animated resourcepack you can check 
    on: 
    https://minecraft.fandom.com/wiki/Tutorials/
    Creating_a_resource_pack . 
---------------------------------------------------------------------13. If you have a trouble shooting, that if you compress your   
    texturepack and you drag the .zip file into the minecraft  
    resourcepack options and it does not work, you get an error 
    message on the top right and the texture look the same like in 
    vanilla minecraft, you have to go to the terminal and type: "cd 
    [Where your resourcepack folder is stored]" and then straight 
    into your resourcepack, by typing: "cd [The name of your 
    resourcepack folder]". And lastly zip that, by typing: 
    "zip -r ../ [What you want to call it].zip pack.mcmeta assets".
---------------------------------------------------------------------
14. If you have any extra trouble shooting, you may 
    search on the web, because thats 
    what I did, when i was trouble shooting -_- .
---------------------------------------------------------------------
Extra notes: -all folder names have to be lowercase
             -zip contents only, not the folder with the            
              instructions in 13
             -confirm PNG files are valid
             -use ""pack_format" 64; for MC 1.21.x


This whole thing is based on the instructions of
https://minecraft.fandom.com/wiki/Tutorials/Creating_a_resource_pack,
so in case you have any questions or want more info please look there or write in my github comments.
      
