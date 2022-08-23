
# Piranha Naming Implementation 

The Piranha Naming Implementation module delivers you with JNDI implementation.

Add the following dependency to your project to use it.

      <dependency>
          <groupId>cloud.piranha.naming</groupId>
          <artifactId>piranha-naming-impl</artifactId>
          <version>x.y.z</version>
      </dependency>

And then you either will have to pass in the InitialContextFactory using a property

      -Djava.naming.factory.initial=cloud.piranha.naming.impl.DefaultInitialContextFactory

or programmatically set it:

      System.getProperties().put("java.naming.factory.initial", 
        "cloud.piranha.naming.impl.DefaultInitialContextFactory");

Note that this example does not set the &lt;scope&gt; but depending on what you
are using Piranha Naming for you might need to add a &lt;scope&gt;.
