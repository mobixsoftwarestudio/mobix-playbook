# Our References

## References

Everything we wrote comes from our experiences, good practices exchanges, professional knowledge and, especially, from books that inspired us.  


* How to Win Friends and Influence People \(Dale Carnegie\) - He says you can make someone want to do what you want them to by seeing the situation from the other person's point of view and “ arousing in the other person an eager want””. This is a Bible for us because we learnt how to make people like you, win people over to your way of thinking, and change people without causing offense or arousing resentment.
* Measure What Matters \(John Doerr\) - We discovered how a powerful goal-setting system is essential to grow, since it has helped tech giants such as Google and Intel to exceed all expectations. It taught us to structure an organization that thrives by setting OKRs as the basis of the whole playbook. Finally, we understood the importance of culture and of a continuous performance management.
* Find Your Why \(Simon Sinek\) - This is another fundamental book for us, since the whole concept of WHY is grounded in the tenets of the biology of human decision making. How the Golden Circle works maps perfectly with how the brain works. It taught us that whether you are an entrepreneur, an employee, a leader of a team, or are looking to find clarity on your next move, your WHY is the one constant that will guide you toward fulfillment in your work and life. 
* The Art of Doing Twice the Work in Half the Time \(Jeff Sutherland\) - Scrum is mandatory reading for any leader, whether they’re leading troops on the battlefield or in the marketplace. We understood that success requires tremendous speed, enormous productivity, and an unwavering commitment to achieving results. 
* Dono \(Marcelo Toledo\)- This book is a guide for any entrepreneur who wants to start a startup. Marcelo Toledo, who has been working with startups for over 12 years, has studied all the most modern startup creation techniques, applied and tested each one of them, mixed it with his learning and created his own methodology, which unifies the techniques, putting them to work together and in an order that makes sense. All this thinking about the reality of Brazilian advantages and limitations.
* The Hard Thing About Hard Things \(Ben Horowitz\) - The author draws on his own story of founding, running, selling, buying, managing, and investing in technology companies to offer essential advice and practical wisdom for navigating the toughest problems business schools don't cover. A lifelong rap fan, Horowitz amplifies business lessons with lyrics from his favorite songs and tells it straight about everything from firing friends to poaching competitors, from cultivating and sustaining a CEO mentality to knowing the right time to cash in.
* Value Proposition Design: How to Create Products and Services Customers Want \(A. Osterwalder, Y. Pigner, G. Bernarda, A. Smith\) - It helped us tackle the core challenge of every business, by creating compelling products and services customers want to buy.
* Clean Code: A Handbook of Agile Software Craftsmanship \(Robert C. Martin\) - Even bad code can function. But if code isn’t clean, it can bring a development organization to its knees. Every year, countless hours and significant resources are lost because of poorly written code. But it doesn’t have to be that way. This book is a must for any developer, software engineer, project manager, team lead, or systems analyst with an interest in producing better code.
* **Websites references:** 
  * * [**http://www.uxforthemasses.com/ux-manifesto/**](http://www.uxforthemasses.com/ux-manifesto/)
    * [**https://agilemanifesto.org/**](https://agilemanifesto.org/)
    * [**https://medium.com/**](https://medium.com/)
    * [**http://es6-features.org/**](http://es6-features.org/#Constants)[**\#Constants**](http://es6-features.org/#Constants)

These references taught us something that lives on in our culture. Sometimes bringing us things we haven’t ever heard of, and other times just by asserting things we already had stumbled upon in our practice and use frequently in our day-to-day.

{% api-method method="get" host="https://api.cakes.com" path="/v1/cakes/:id" %}
{% api-method-summary %}
Get Cakes
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" %}
ID of the cake to get, for free of course.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="recipe" type="string" %}
The API will do its best to find a cake matching the provided recipe.
{% endapi-method-parameter %}

{% api-method-parameter name="gluten" type="boolean" %}
Whether the cake should be gluten-free or not.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```
{    "name": "Cake's name",    "recipe": "Cake's recipe name",    "cake": "Binary cake"}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```
{    "message": "Ain't no cake like that."}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



