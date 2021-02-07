Account

public class Account{
	protected String accName;
	protected String acId;
	protected int balance;
	
	Account(){
	}
	
	Account(String accName,String acId,int balance){
		this.accName=accName;
		this.acId=acId;
		this.balance=balance;	
	}
	
	public void deposit(int amount){
		if(amount<0){
			Console.WriteLine("Amount can not be negative");
		}
		else{
		balance=balance+amount;
		Console.WriteLine("Deposited Money: " +amount);
		}
	}

	public void Withdraw(int amount){
		if(balance>=amount){
			balance=balance-amount;
			Console.WriteLine("Withdrawal Money: " +amount);
		}
		else
		{ Console.WriteLine("Insifficient Balance");
		}
	}
	/*public void checkBalance(){
		Console.WriteLine("Current Balance:" +balance);
	}*/
	
	
}
