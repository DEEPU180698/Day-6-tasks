DAY 6 TASKS

Task 1
1.Write a “person” class to hold all the details.
class person {
    constructor(name, age, gender, email, mobile_number, city, country) {
      this.name = name
      this.age = age
      this.gender = gender
      this.email = email
      this.mobile_number = mobile_number
      this.city = city
      this.country = country
    }
    getName() {
      return this.name
    }
    getAge() {
      return this.age
    }
    getGender() {
      return this.gender
    }
    getEmail() {
      return this.email
    }
    getMobileNumber() {
      return this.mobile_number
    }
    getCity() {
      return this.city
    }
    getCountry() {
      return this.country
    }
    setName(name) {
      this.name = name
    }
    setAge(age) {
      this.age = age
    }
    setGender(gender) {
      this.gender = gender
    }
    setEmail(email) {
      this.email = email
    }
    setMobileNumber(mobile_number) {
      this.mobile_number = mobile_number
    }
    setCity(city) {
      this.city = city
    }
    setCountry(country) {
      this.country = country
    }
  }
  
  const person1 = new person("Deepu",25,"male","deepu@gmail.com",9293229922,"Tirunelveli","TN")
  const person2 = new person("Ashok",24,"male","ashok@gmail.com",7772228733,"Kollam","KL")
  console.log(person2.getName()) 
  console.log(person1.getCity()) 
person2.setCity("Tirunelveli")
console.log(person2.getCity())  
person1.setName("Deepu")
console.log(person1.getName())  


TASK 2

class UberPriceCalc{
    constructor(distInKms, timeInMins){
        this.distanceInKms=distInKms
        this.timeInMins=timeInMins
        this.baseFare=10  
        this.costPerKms=3  
        this.costPerMins=1  
    }

    calculatePrice(){
         const distanceCost = this.distanceInKms * this.costPerKms;
         const timeCost = this.timeInMins * this.costPerMins;
         const totalCost = this.baseFare + distanceCost + timeCost;
         return `$${totalCost.toFixed(2)}`;
    }
}

let distance = 17 
let time = 38 
let ride = new UberPriceCalc(distance,time)
console.log(`The cost of the ride is ${ride.calculatePrice()}`)


