Роботу виконав студент групи ІО-14 Подлубний Максим. Так як в мене немає STM32 Discovery з виходом 3,5 Mini Jack я зробив іншу роботу.  
В мене є дві плати, до першої-- STM32 Nucleo під'єднаний джойстик, плата читає з нього значення і передає їх по інтерфейсу I2C, вона виконує роль Master, на іншому кінці під'єднана плата STM32 BlackPill до якої в свою чергу під'єднані чотири світлодіоди, коли я повертаю джойстик в одну з сторін світиться відповідний світлодіод.  
Джойстик працює на двох потенціометрах виводи яких підключені до ADC пінів PA1, PA2, їх значення отримує плата Nucleo і як Master передає по інтерфейсу I2C до плати BlackPill.