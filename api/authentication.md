# Authentication

{% api-method method="post" host="http://api-oversight.in" path="/api/auth/signup/" %}
{% api-method-summary %}
Sign Up
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to sign up and create an account on Oversight.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-form-data-parameters %}
{% api-method-parameter name="username" type="string" required=true %}
The username that you would like to create the account under.
{% endapi-method-parameter %}

{% api-method-parameter name="email" type="string" required=true %}
The email-id you would like to link to your account.
{% endapi-method-parameter %}

{% api-method-parameter name="password" type="string" required=true %}
The password to authenticate your account in the future
{% endapi-method-parameter %}

{% api-method-parameter name="confirm\_password" type="string" required=true %}
Confirm the password you entered
{% endapi-method-parameter %}

{% api-method-parameter name="first\_name" type="string" required=true %}
Your first name
{% endapi-method-parameter %}

{% api-method-parameter name="last\_name" type="string" required=true %}
Your last name
{% endapi-method-parameter %}
{% endapi-method-form-data-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=201 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Confirmation Mail Has Been Sent",
    "username": "Your username",
    "email": "Your email"
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=400 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "detail": "Email could not be sent, please check your email-id and try again"
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



