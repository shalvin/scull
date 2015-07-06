# scull
A character device driver that acts on a memory area as if it were a device.
Scull is short for Simple Character Utility for Loading Localities. scull is a char driver that acts on a memory area as though it were a device. A side effect of this behavior is that, as far as scull is concerned, the word device can be used interchangeably with "the memory area used by scull."
The advantage of scull is that it isn't hardware dependent, since every computer has memory. scull just acts on some memory, allocated using kmalloc. Anyone can compile and run scull, and scull is portable across the computer architectures on which Linux runs. On the other hand, the device doesn't do anything "useful" other than demonstrating the interface between the kernel and char drivers and allowing the user to run some tests.

This is a university project - see http://www.xml.com/ldd/chapter/book/ch03.html for information.