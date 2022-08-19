# delegation-ctf
we can mess around with delegation through a fallback

The contract is using delegation in the wrong way which means we can trick the data that is stored there. It's also vulnerable to a fallback.
 In this case we can make a transfer to the contract address using incorrect data to trick the contract since 

  function pwn() public {
    owner = msg.sender;
  }
this function is part of the contract then it should make us the owner, and it does!
