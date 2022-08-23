
# Manorrock Herring - Thread

The Manorrock Herring - Thread module delivers you with ThreadLocal JNDI implementation.

Add the following dependency to your project to use it.

      <dependency>
          <groupId>com.manorrock.herring</groupId>
          <artifactId>herring-thread</artifactId>
          <version>x.y.z</version>
      </dependency>

And then you either will have to pass in the InitialContextFactory using a property

      -Djava.naming.factory.initial=com.manorrock.herring.thread.ThreadInitialContextFactory

or programmatically set it:

      System.getProperties().put("java.naming.factory.initial", 
        "com.manorrock.herring.thread.ThreadInitialContextFactory");

Note that this example does not set the &lt;scope&gt; but depending on what you
are using Manorrock Herring - THread for you might need to add a &lt;scope&gt;.
