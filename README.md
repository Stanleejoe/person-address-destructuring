# person-address-destructuring
const people = [  
    { name: "Alice", address: { city: "New York", street: "Broadway", number: 123 } },  
    { name: "Bob", address: { city: "Los Angeles", street: "Sunset Boulevard", number: 456 } }  
];  

const result = people.map(({ name, address: { city, street } }) => {  
    return `${name} lives in ${city} on ${street}.`;  
});  

console.log(result);
