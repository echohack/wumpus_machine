# wumpus_machine

![Discord tweet](/docs/discord.png)

Well I guess I could do something completely unnecessary.

> ...Well on second thought, let's not go Camelot. It tis a silly place.

Let's launch a Windows 2016 machine in AWS with `AWS Nitro`. That's like Discord Nitro... right? (Who can keep up with all of these AWS product names anyway?! WHAT THE HELL IS AWS ELASTIC BEANSTALK? For Wumpus's sake, AWS Glue?!? AHHHHH!)

## Usage

1. Install [terraform](https://releases.hashicorp.com/terraform/). You'll need version 0.11.14, because I haven't converted this to 0.12.0 yet. No, I don't know why Hashicorp still hasn't made Terraform version 1.0.0+ even though it's five years old now. Yes, I agree with you, 0.12.0 should be a major release, because semantic versioning and... can we just get on with this?

2. Rename `example.tfvars` to `terraform.tfvars`. You'll need to fill it out with your own AWS information.

3. Run Terraform from the `terraform` directory as so:

Warning: If you've never used AWS before, this will cost you real money!

- `terraform init`
- `terraform plan`
- `terraform apply`

4. Discord will automatically install and launch itself. You don't even need to interact with anything. I guess you could use Microsoft Remote Desktop and connect using the information that is auto-generated at the end of the Terraform run. The Terraform run will output the public ip address, and the randomly generated password for the Administrator account.

The whole run should take about 5 minutes.

5. Well that was silly, so let's be done with this already.

- `terraform destroy -auto-approve`

## Testing

Who do you think I am, some kind of software engineer?!

Fine. I took a screenshot of the RDP session after the run succeeded. Is this enough?

![Image of RDP](/docs/rdp.png)


