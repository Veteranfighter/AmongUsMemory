# AmongUsMemory

**Working Fine 2020.8.12s**

**It only works with the version downloaded from Steam!**

## How to Use
 1. Download Source Code
 2. Add Reference AmongUsMemory Your Project 
 3. End
 
 
### Example Code
 ```cs
        static void Main(string[] args)
        {
            var isAmongUsRunning = HamsterCheese.AmongUsMemory.Cheese.Init();
            if(isAmongUsRunning)
            {
               var players = HamsterCheese.AmongUsMemory.Cheese.GetAllPlayers();

               Console.WriteLine("Test Read Player Datas..");
               while (true)
               {
                   foreach (var data in players)
                   {
                       Console.WriteLine("find player color : " + data.PlayerInfo.Value.ColorId);
                       Console.WriteLine("find player position : " + data.GetSyncPosition().x + "," + data.GetSyncPosition().y);
                   }

               }
               System.Threading.Thread.Sleep(1000000);
            }
        }
 ```

### Read String Pointer
 Call Utils.ReadString(offset);
 
 
You can get all player info ( IsImposter / IsDead / Position .. etc )

## Example Cheat

 this is my private cheat
 ![](https://github.com/shlifedev/AmongUsPublic/blob/master/Example.PNG) 
 https://www.youtube.com/watch?v=Cfk9_wNjEto&feature=youtu.be
 
 
Just use it for study purposes only.


## TODO

 full automatic cheating (detect map, detect new game.. etc)
 currently require restart cheat every game.
 
## PatchNotes

 * 2020-08-26 -- added **readString** function in Utils.cs. now you can read string pointers.
 * 2020-08-24 -- added **getShipstatus** function in cheese.cs
 * 2020-08-20 -- fix wrong data structure
 * 2020-08-20 -- added auto structure generator xml based
 
