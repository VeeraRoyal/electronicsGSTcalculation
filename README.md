# electronicsGSTcalculation
calculate GST
import os
class Goods:
    Electronics=[]
    def myElectronics(self,Electronics):
        electronics = input("enter the item")
        Electronics.append(electronics)
        print(Electronics)
        os.chdir("c://Goods")
        myfile1=open("c://Goods//Electronics.txt","a+")
        myfile1.write(str(Electronics))
        myfile1.close()
        if electronics=="tv":
            tvexpectedPrice=int(input("Enter Your prize to Buy the tv :"))
            if tvexpectedPrice >=5000:
                tvGST=tvexpectedPrice*0.01
                print("5000 TV GST is :",tvGST)
                os.chdir("c://Goods") 
                myfile1 = open("c://Goods//Electronics.txt", "a+")
                myfile1.write(str(tvGST))
                myfile1.close()
            else:
                print("tv cost is more than 5000")
        elif electronics=="fridge":
            fridgeExpectedPrice=int(input("Enter your price to buy a fridge :"))
            if fridgeExpectedPrice >=10000:
                fridgeGST=fridgeExpectedPrice*0.01
                print("fridge GST is :",fridgeGST)
                os.chdir("c://Goods")
                myfile1 = open("c://Goods//Electronics.txt", "a+")
                myfile1.write(str(fridgeGST))
                myfile1.close()
            else:
                print("item are not matching in this range")
        elif electronics=="mobile":
            mobileExpectedPrice = int(input("Enter your price to buy a fridge :"))
            if mobileExpectedPrice >= 5000:
                mobileGST = mobileExpectedPrice * 0.01
                print("mobile GST is :", mobileGST)
                os.chdir("c://Goods")
                myfile1 = open("c://Goods//Electronics.txt", "a+")
                myfile1.write(str(mobileGST))
                myfile1.close()
            else:
                print("item are not matching in this range")
        elif electronics=="laptap":
            laptapExpectedPrice = int(input("Enter your price to buy a laptap :"))
            if laptapExpectedPrice >= 5000:
                laptapGST = laptapExpectedPrice * 0.01
                print("mobile GST is :", laptapGST)
                os.chdir("c://Goods")
                myfile1 = open("c://Goods//Electronics.txt", "a+")
                myfile1.write(str(laptapGST))
                myfile1.close()
            else:
                print("item are not matching in this range")
        elif electronics=="washingmachine":
            washingmachineExpectedPrice = int(input("Enter your price to buy a washingmachine :"))
            if washingmachineExpectedPrice >= 5000:
                washingmachineGST = washingmachineExpectedPrice * 0.01
                print("mobile GST is :", washingmachineGST)
            else:
                print("item are not matching in this range")

        else:
            print("entered item is not matching in the electronics")


myobj=Goods()
electronics1=list()
myobj.myElectronics(electronics1)
