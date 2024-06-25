#include "Fire.h"
#include <iostream>

Fire::Fire() : burning(false) {}

void Fire::ignite() {
    if (!burning) {
        burning = true;
        std::cout << "The fire has been ignited!" << std::endl;
    } else {
        std::cout << "The fire is already burning." << std::endl;
    }
}

void Fire::extinguish() {
    if (burning) {
        burning = false;
        std::cout << "The fire has been extinguished." << std::endl;
    } else {
        std::cout << "The fire is already out." << std::endl;
    }
}

bool Fire::isBurning() const {
    return burning;
}
