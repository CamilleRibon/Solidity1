// public variables here
   string public tokenName = "Camille";
   string public tokenAbbrv = "Cam";
   uint public totalSupply = 0;
// mapping variable here
   mapping  (address => uint) public balances;
// mint function
   function mint (address _address, uint _value)public {
if(balances[_address] >= _value){
    totalSupply -= _value;
    balances[_address] -= _value;
    } }

// burn function
