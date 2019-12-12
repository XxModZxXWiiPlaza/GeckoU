# GeckoU
Gecko U is a .NET Framwork library for [BullyWiiPlaza's TCP Gecko](https://github.com/BullyWiiPlaza/tcpgecko)

# Installation

The Installation for this is very simple for this. All you will need to do is drag and drop this into your project and you will be able to reference this in your class. 


# Examples  
Same code that is used to show off [SharpGck](https://github.com/kzpns/ShpGck) ported to GeckoU
```c-sharp
using System;
using com.wiiplaza.geckou;
namespace Gecko_U_Show_Off
{
    class Program
    {

        public static GeckoUCore GeckoU;
        public static GeckoUConnect GeckoUConnection;

        static void Main(string[] args)
        {

            Console.Write("Wii U's IPv4> ");
            string ip_addr = Console.ReadLine();

            GeckoU = new GeckoUCore(ip_addr);

                Console.WriteLine("Connecting tcpgecko server...");
                GeckoU.GUC.Connect();
                Console.WriteLine("Connected!");

                Console.WriteLine("Sending codes...");
                GeckoU.WriteUInt(0x1004F71C, 0); //Home Button Menu Anywhere [Macopride64])
                Console.WriteLine("Sent!");
                Console.WriteLine("You can use the Home Menu in anywhere.");
                GeckoU.GUC.Disconnect();
                Console.ReadKey(false);
        }
    }
}
```

# Credits 

- ```SlothWiiPlaza```: Development 
- ```XxModZxXWiiPlaza```: Development
- ```BullyWiiPlaza```: Development
- Can't remember who all worked on/where Sloth got the orignal code from if you find your code in here people let me know and I will add you to the credits

# Notes

If you are to use this TCP Gecko library in your project all people above must be credited or WiiPlaza(or WiiPlaza Inc.) if using without credit you are subject to have your software removed from where it is hosted. You are to use this and credit all people involved in development. 
You also can not edit the code without permission as well 


*WiiPlaza Inc. Copright 2019*
        
