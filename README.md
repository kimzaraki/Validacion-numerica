#include<iostream>
#include<limits>
int main(){
	int age{};
	while(true){
		std::cout<<"ingrese su edad: ";
		std::cin>>age;
		
		if(std::cin.fail()){
			std::cin.clear();
			std::cin.ignore(std::numeric:limits<std::streamsize>::max(),'\n') ;
			continue;
		}
		if (age<=0){
			continue;
			break;
		}
	}
	std::cout<<"ingresaste: "<<age<<'\n';
}
