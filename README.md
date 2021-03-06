# EMAC Library for TAIJIUINO Due Pro R2

[![TAIJIUINO Due Pro R2 ethernet](http://www.elechouse.com/elechouse/images/product/TAIJIUINO%20DUE%20R2/Taijiuino%20R2-7.jpg)](http://www.elechouse.com/elechouse/index.php?main_page=product_info&cPath=72_73&products_id=2230&zenid=9mdii7ejo1nv94qu2ldalhbp30)

This library is used to test the EMAC function of **TAIJIUINO Due Pro R2**.

##Note##

This library is develop by [Palliser](http://forum.arduino.cc/index.php?PHPSESSID=bbd7atuo3331b4hiqei9ivf4r3&action=profile;u=148087) from Arduino forum, and it is not the final version. [Forum Discussion](http://forum.arduino.cc/index.php?PHPSESSID=9jo0108im6j0sc2bm0mndvbgq7&topic=142908.0).

*[Palliser's github](https://github.com/Palliser), Palliser think the code is not perfect enough, so he didn't upload these codes at present.*

*We upload it here just want to make a demo to our users.*

## How To ##

1. *Place*
	emac.h rstc.h ---->   ...\arduino-1.5.2-windows\arduino-1.5.2\hardware\arduino\sam\system\libsam\include
   
	emac.c rstc.c ---->   ...\arduino-1.5.2-windows\arduino-1.5.2\hardware\arduino\sam\system\libsam\source *respectively*

	variant.cpp and variant.h ---> ...\arduino-1.5.2-windows\arduino-1.5.2\hardware\arduino\sam\variants\arduino\_due\_x, **arduino\_due\_x** folder alread have variant.cpp and variant.h, you need replace them, back up first. 

	*emac.h, rstc.h, emac.c, rstc.c, variant.cpp and variant.h are in CopyToAnotherDir*

1. Copy **EMAC** folder to **$ArduionScketch/libraries**

1. Connect **DUE Ethernet Module** with **TAIJIUINO Due Pro R2**, open example **Arduino\_Due\_EMAC\_Mod**, upload it to **TAIJIUINO Due Pro R2**. 

1. Set your PC ip address to **192.168.0.3**, submask **255.255.255.0**, gate way **192.168.0.1**. Connect your PC and **DUE Ethernet Module** through network cable. Restart your **TaijiDue**, wait for the connection is established.
	Ping 192.168.0.2, and the result:

	![ping result](./image/ping.jpg)