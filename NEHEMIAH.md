# Cmp114Project
class SavingsAccount(Account):

    def __init__(self, account_number, balance=0, interest_rate=0.0):

        super().__init__(account_number, balance)

        self.interest_rate = interest_rate

    def apply_interest(self):

        interest = self.balance * self.interest_rate

        self.balance += interest

        return True
