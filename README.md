# Ethereum-truffle-items
Some err happened when I have tried which described solution


When we meet the errors: No network specified. Cannot determine current network. 
Solution:

just import these code into the truffle.js 

module.exports = {
   networks: {
        development: {
            host: "localhost",
            port: 8545,
            network_id: "*" // 匹配任何network id
         }
    }
};

And then we'll meet the situations that miss Metacoin contract, the following is solution:

We create a new empty directory name metacoin and terminal input the command ：turffle unbox metacoin



Finally, we also meet "there is no app in the metacoin". Solution like above operation：

The directory name app and terminal input the command ：turffle unbox tutorialtoken.

PS: this is a virtual currency demo. Good luck!
