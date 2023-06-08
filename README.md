# HokieBot Code
// The HMC5583L compass must be connected and working in order for the sketch
to work properly
// If you are having problem, Check the I2C address of the compass, mine is 0x1E
// You may need to connect the compass to the Arduino and run a I2C Scanner Sketch to check the I2C address
// The HMC5883L chip used in the compass module has a fixed I2C address of 0x1E. 
// This means that the Jarzebski HMC5883L library assumes that the compass module is connected to the I2C bus with this address, 
// and the library's code is written accordingly.
// In the library's source code, you can find the line that sets the I2C address to 0x1E in the HMC5883L.h header file:
// #define HMC5883L_I2CADDR 0x1E
// This sets the I2C address to 0x1E, which is the default address of the HMC5883L chip used in the compass module.
// If your compass module has a different I2C address (for example, if it has been modified to use a different address), 
// you can modify this value in the header file to match the address of your module. 
// In that case, you need to upload the modified library to the Arduino board in order to use it.
