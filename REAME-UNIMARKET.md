## Unimarket Versioned Querydsl

**Change by Unimarket team**

Clone from master Querydsl 4.2.1

* merge the pull request [https://github.com/querydsl/querydsl/pull/2283](https://github.com/querydsl/querydsl/pull/2283) to resolve Hibernate 5.3 compatibility
* change "com.querydsl.jpa.hibernate.HibernateUtil" to set query parameter by ordinal parameter instead of by named parameter, because hibernate 5.3 does not support it any more. 

After Querydsl upgrades to support hibernate 5.3, we could verify Unimarket app function and use public version of Querydsl.  

**How to deploy it to JFrog Artifactory**

mvn deploy -Dusername={username} -Dpassword={password} -Dbuildnumber={buildnumber}

