# PetaLinux Environment Creation using Zynq UltraScale+ MpSoc
In a world where technology seamlessly intertwines with our daily lives, embedded systems stand as the unsung heroes, quietly powering the devices we rely on every day. These systems, blending hardware and software intricately, bring forth a symphony of functionality, efficiency, and innovation. At the heart of this realm lies embedded Linux, an agile and open-source operating system shaping the very core of modern embedded devices, offering a playground of customization and scalability.


Enter the Zynq UltraScale+ MPSoC, a beacon of computational prowess, seamlessly merging processing capabilities and programmable logic to deliver a powerhouse fit for complex embedded applications. From automotive advancements to IoT marvels, this platform stands tall, driving innovation across industries with its versatility and performance.

As we embark on a journey into the depths of FPGA development, we set our sights on Vivado 2019.2, a gateway to crafting a small RTL project with precision and finesse. Our canvas expands further as we delve into the intricate process of setting up Ubuntu 18.04.2, paving the way for seamless integration of tools and frameworks crucial for our endeavor. Alongside, Petalinux 2019.2 beckons, offering a realm of possibilities in shaping a tailored Linux environment to suit our project's unique demands.


In a world where technology seamlessly intertwines with our daily lives, embedded systems stand as the unsung heroes, quietly powering the devices we rely on every day. These systems, blending hardware and software intricately, bring forth a symphony of functionality, efficiency, and innovation. At the heart of this realm lies embedded Linux, an agile and open-source operating system shaping the very core of modern embedded devices, offering a playground of customization and scalability.

Enter the Zynq UltraScale+ MPSoC, a beacon of computational prowess, seamlessly merging processing capabilities and programmable logic to deliver a powerhouse fit for complex embedded applications. From automotive advancements to IoT marvels, this platform stands tall, driving innovation across industries with its versatility and performance.

As we embark on a journey into the depths of FPGA development, we set our sights on Vivado 2019.2, a gateway to crafting a small RTL project with precision and finesse. Our canvas expands further as we delve into the intricate process of setting up Ubuntu 18.04.2, paving the way for a seamless integration of tools and frameworks crucial for our endeavor. Alongside, Petalinux 2019.2 beckons, offering a realm of possibilities in shaping a tailored Linux environment to suit our project's unique demands.


Within the confines of memory limitations, we navigate the delicate dance of resource optimization on the Zynq UltraScale+ MPSoC, seeking to maximize efficiency while ensuring peak performance. As we tread this path, we unravel the complexities of embedded systems, each step bringing us closer to a world where innovation meets execution with precision.

Join us as we embark on this enlightening odyssey, where the convergence of technology and creativity paints a canvas of possibilities waiting to be explored.



<p align="center"><img src="medium/Screenshot from 2024-01-28 10-03-12.png" width="480"\></p> 

<p align="center"><img src="medium/Screenshot from 2024-01-28 10-04-52.png" width="480"\></p>

Installing Ubuntu on a virtual environment is also okay, but there are some complications ahead. For example, we cannot use the system file folder in Vitis. If we want to create a Linux platform and run an application in Petalinux, we have to complete the application program in the platform that we create in Vitis. At that time, we have to use the created Petalinux system folder. We cannot access that folder which is in Virtualbox to Windows.

So we have to install everything - Vivado, Vitis, along Petalinux - in the Ubuntu environment itself. Even after this, there will be complications. Creating and running a Vivado project in Virtualbox is not easy, especially if the project is big. In that case, we need a much larger memory size, such as good RAM, to run and create the Bitstream file.

In my opinion, installing everything (Vivado, Vitis, Petalinux, etc.) on a separate Ubuntu desktop is much better than Virtualbox. We have to carefully follow the installation guide before installation itself, or it will be a very time-consuming process later.

Again, Petalinux and Vivado Vitis are interrelated. If we are using Vivado 2019.2, then we have to install Petalinux 2019.2 only, not any other version. Installing Vivado on Ubuntu is version-specific so we have to go through every line of the Vivado installation guide before installing Ubuntu itself to avoid unnecessary time waste.

In my context, I used Vivado version 2019.2. In the installation guide of Vivado and even the Petalinux guide, we can see that only the Ubuntu 18.04.2 version is very compatible to work with. So we have to install only that particular version, not any other like 2020.04.2 or any other generalized version of Ubuntu 18.04. This may later install the final version of its type, which may cause Vivado to not run properly.

Installing Petalinux 2019.2 is very critical. For this, we have to select only English as the OS language. Operating systems with other languages are not suitable for Petalinux. If you want the step-by-step guide of Petalinux installation, you can redirect to this page.
