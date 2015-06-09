## Directive template -
## exemple validation

    <form name='loginForm'>
           <input name='login' required type='email' ng-model='user.login'/>
           <span ng-show='loginForm.login.$dirty &&
           loginForm.login.$error.required'>A login is required</span>
           <span ng-show='loginForm.login.$error.email'>
           Your login should be a valid email</span>
           <input name='password' ng-model='user.password'/>
    </form>
