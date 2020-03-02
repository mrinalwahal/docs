---
description: We follow a compartmentalised payout model.
---

# Payouts

## Deadlines

Maximum 6 months, from the date of publishing of project, is the default deadline of every project for every Rs. 1,00,000 compartment of total target.

* For targets up to 1,00,000, deadline is 6 months maximum.
* Similarly, 12 months for targets up to 2,00,000.
* And so on, until a maximum target value of Rs. 25,00,000.

{% hint style="info" %}
Since, deadlines are decided upon compartments rounded of to Rs. 1,00,000, **deadline for a hypothetical target of Rs. 1,20,000 would also be 12 months.**
{% endhint %}

{% hint style="danger" %}
1. Deadlines are not changeable.
2. You won't get any portion of your raised money if you missed your given deadline.
{% endhint %}

## Disbursement

Oversight automatically disburses funds lower than 1,00,000 in one-go. And for targets beyond 1,00,000, we disburse in instalments of 50,000 each.

Pseudo-Code used:

```text
if target_amount <= 100000 
		and collected_amount == target_amount: 
					APPROVE disbursement
		
	else:
		if (collected_amount - already_disbursed_amount) >= 50000 
					and collected_amount <= target_amount:
					APPROVE disbursement

		else: BLOCK disbursement
```

| Test Case 1 |  |
| :--- | :--- |
| Collected | 20,000 |
| Target | 1,20,000 |
| Disbursement | Disproved |
| Reason | Need to touch 1,00,000 for first instalment |

| Test Case 2 |  |
| :--- | :--- |
| Collected | 1,00,000 |
| Target | 1,00,000 |
| Disbursement | Approved |

| Test Case 3 |  |
| :--- | :--- |
| Collected | 80,000 |
| Target | 80,000 |
| Disbursement | Approved |
| Reason | Since, target is below 1,00,000, all collected funds are disbursed in single instalment. |

| Test Case 4 |  |
| :--- | :--- |
| Collected | 1,10,000 |
| Already Disbursed | 1,00,000 |
| Target | 1,20,000 |
| Disbursement | Disproved  |
| Reason | Now funds can only be disbursed upon touching final target of 1,20,000. |

You shall automatically receive a congratulatory email from Oversight within 48 hours of you hitting your funding target, on a per project basis. This email shall mark that we have acknowledged your target is achieved and have initiated the final disbursement of all your funds.

{% hint style="warning" %}
How long it takes for funds to be deposited in your account also depends on your bank's processing time. Also, is must be clear that **no payouts are issued on bank/national/regional holidays in India.**
{% endhint %}

{% hint style="danger" %}
_Disclaimer: Oversight only supports sponsorship for projects published by **Indian residents**, therefore, if you have mistakenly been allowed to raise funds for your project despite not being an Indian resident/citizen \(unless Oversight has issued announcements for international operations\), Oversight is not responsible for disbursing your funds, since it goes against our policies. **You have been warned.**_
{% endhint %}

## Preferred Account

Your bank account will be the preferred option for initiating payouts to, since VPA \(UPI\) accounts have an upper limit on transactions as per governmental regulations. However, if the total payout falls within the permitted transaction limit specified by the Government of India, or Reserve Bank of India \(RBI\), then VPA account shall be preferred for the payout.

Therefore, it is advised to have your bank account attached as the funding account on your Oversight profile, to make things easier and safer. 

## Halting Disbursements

Oversight is currently updating it's policy on what kind of projects, or projects pertaining to which field, what intentions and/or what objectives will be allowed to be published and funded on its platform. As of now, there is no restriction on which kind of projects can be funded. It's an open ground and a wild west for every passionate researcher/developer out there.

However, Oversight reserves the right to un-publish or delete any project from its platform if it seems problematic to Oversight. These could projects pertaining to Weapons Engineering, or dangerous neuro-scientific experimentation, amongst others. 

Beyond that, Oversight also reserves the right to block or permanently halt disbursements i.e. decide against disbursing collected/raised funds by any user/author on any of their projects, for reasons pertaining to errors in documentation or records maintained that of the user or their projects. Easiest way to negotiate the release of funds with Oversight in such a scenario is to comply with any/every recovery methods that Oversight describes to users in that case.

