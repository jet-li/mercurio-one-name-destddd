Hola Rafa..Hay un error al levantar procesos automaticos

> at weblogic.jms.extensions.JMSDestinationAvailabilityHelper$DestinationAvailabilityListenerWrapper.onDDMembershipChange(JMSDestinationAvailabilityHelper.java:372)
> > at weblogic.jms.common.CDS$DD2Listener.run(CDS.java:1237)
> > at weblogic.work.SelfTuningWorkManagerImpl$WorkAdapterImpl.run(SelfTuningWorkManagerImpl.java:528)
> > at weblogic.work.ExecuteThread.execute(ExecuteThread.java:207)
> > at weblogic.work.ExecuteThread.run(ExecuteThread.java:176)
Caused By: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'applicationContext-main' defined in URL [zip:/filestore/Dagobah/servers/w76sNPDABatch/tmp/_WL\_user/despaduanero2-declaracion-ingreso-batch\_2.10.0/p02spp/lib/despaduanero2-ingreso-batch.jar-2.10.0.jar!/beanRefContext.xml]: Instantiation of bean failed; nested exception is org.springframework.beans.BeanInstantiationException: Could not instantiate bean class [pe.gob.sunat.framework.spring.context.IgnoreDuplicateImportsClassPathXmlApplicationContext]: Constructor threw exception; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'ValidadorVehiculoService': Injection of autowired dependencies failed; nested exception is org.springframework.beans.factory.BeanCreationException: Could not autowire field: private pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios pe.gob.sunat.despaduanero2.declaracion.ingreso.validador.formatob.descrminimas.service.ValidadorVehiculoServiceImpl.fabricaDeServicios; nested exception is org.springframework.beans.factory.NoUniqueBeanDefinitionException: No qualifying bean of type [pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios] is defined: expected single matching bean but found 10: framework.fabricaDeServicios,catalogo.fabricaDeServicios,manifiesto.fabricaDeServiciosData,transbordo.fabricaDeServiciosData,tramite.fabricaDeServiciosData,exigibilidad.framework.fabricaDeServicios,prevcontrabando2.fabricaDeServicios,manifiesto.fabricaDeServicios,seleccion.fabricaDeServicios,sigad.despacho.entrada.fabricaDeServiciosData
> > at org.springframework.beans.factory.support.ConstructorResolver.autowireConstructor(ConstructorResolver.java:288)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.autowireConstructor(AbstractAutowireCapableBeanFactory.java:1045)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBeanInstance(AbstractAutowireCapableBeanFactory.java:949)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:487)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:458)
> > at org.springframework.beans.factory.support.AbstractBeanFactory$1.getObject(AbstractBeanFactory.java:295)
> > at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:223)
> > at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:292)
> > at org.springframework.beans.factory._

onAvailabilityHelper.java:372)

> at weblogic.jms.common.CDS$DD2Listener.run(CDS.java:1237)
> at weblogic.work.SelfTuningWorkManagerImpl$WorkAdapterImpl.run(SelfTuningWorkManagerImpl.java:528)
> at weblogic.work.ExecuteThread.execute(ExecuteThread.java:207)
> at weblogic.work.ExecuteThread.run(ExecuteThread.java:176)
Caused By: org.springframework.beans.BeanInstantiationException: Could not instantiate bean class [pe.gob.sunat.framework.spring.context.IgnoreDuplicateImportsClassPathXmlApplicationContext]: Constructor threw exception; nested exception is org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'ValidadorVehiculoService': Injection of autowired dependencies failed; nested exception is org.springframework.beans.factory.BeanCreationException: Could not autowire field: private pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios pe.gob.sunat.despaduanero2.declaracion.ingreso.validador.formatob.descrminimas.service.ValidadorVehiculoServiceImpl.fabricaDeServicios; nested exception is org.springframework.beans.factory.NoUniqueBeanDefinitionException: No qualifying bean of type [pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios] is defined: expected single matching bean but found 10: framework.fabricaDeServicios,catalogo.fabricaDeServicios,manifiesto.fabricaDeServiciosData,transbordo.fabricaDeServiciosData,tramite.fabricaDeServiciosData,exigibilidad.framework.fabricaDeServicios,prevcontrabando2.fabricaDeServicios,manifiesto.fabricaDeServicios,seleccion.fabricaDeServicios,sigad.despacho.entrada.fabricaDeServiciosData
> at org.springframework.beans.BeanUtils.instantiateClass(BeanUtils.java:163)
> at org.springframework.beans.factory.support.SimpleInstantiationStrategy.instantiate(SimpleInstantiationStrategy.java:121)
> at org.springframework
> at weblogic.work.ExecuteThread.execute(ExecuteThread.java:207)
> > at weblogic.work.ExecuteThread.run(ExecuteThread.java:176)
Caused By: org.springframework.beans.factory.BeanCreationException: Error creating bean with name 'ValidadorVehiculoService': Injection of autowired dependencies failed; nested exception is org.springframework.beans.factory.BeanCreationException: Could not autowire field: private pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios pe.gob.sunat.despaduanero2.declaracion.ingreso.validador.formatob.descrminimas.service.ValidadorVehiculoServiceImpl.fabricaDeServicios; nested exception is org.springframework.beans.factory.NoUniqueBeanDefinitionException: No qualifying bean of type [pe.gob.sunat.framework.spring.util.factory.FabricaDeServicios] is defined: expected single matching bean but found 10: framework.fabricaDeServicios,catalogo.fabricaDeServicios,manifiesto.fabricaDeServiciosData,transbordo.fabricaDeServiciosData,tramite.fabricaDeServiciosData,exigibilidad.framework.fabricaDeServicios,prevcontrabando2.fabricaDeServicios,manifiesto.fabricaDeServicios,seleccion.fabricaDeServicios,sigad.despacho.entrada.fabricaDeServiciosData
> > at org.springframework.beans.factory.annotation.AutowiredAnnotationBeanPostProcessor.postProcessPropertyValues(AutowiredAnnotationBeanPostProcessor.java:288)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.populateBean(AbstractAutowireCapableBeanFactory.java:1116)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.doCreateBean(AbstractAutowireCapableBeanFactory.java:519)
> > at org.springframework.beans.factory.support.AbstractAutowireCapableBeanFactory.createBean(AbstractAutowireCapableBeanFactory.java:458)
> > at org.springframework.beans.factory.support.AbstractBeanFactory$1.getObject(AbstractBeanFactory.java:295)
> > at org.springframework.beans.factory.support.DefaultSingletonBeanRegistry.getSingleton(DefaultSingletonBeanRegistry.java:223)
> > at org.springframework.beans.factory.support.AbstractBeanFactory.doGetBean(AbstractBeanFactory.java:292)
> > at org.springframework.beans.factory.support.AbstractBeanFactory.getBean(AbstractBeanFactory.java:194)
> > at org.springframework.beans.factory.support.DefaultListableBeanFactory.preInstantiateSingletons(DefaultListableBeanFactory.java:626)
> > at org.springframework.context.support.AbstractApplicationContext.finishBeanFactoryInitialization(AbstractApplicationContext.java:933)
> > at org.springframework.context.support.AbstractApplicationContext.refresh(AbstractApplicationContext.java:479)
> > at org.springframework.context.support.ClassPathXmlApplicationContext.

&lt;init&gt;

(ClassPathXmlApplicationContext.java:139)
> > at org.springframework.context.support.ClassPathXmlApplicationContext.

&lt;init&gt;

(ClassPathXmlApplicationContext.java:94)
> > at pe.gob.sunat.framework.spring.context.IgnoreDuplicateImportsClassPathXmlApplicationContext.

&lt;init&gt;

(IgnoreDuplicateImportsClassPathXmlApplicationContext.java:40)
> > at sun.reflect.NativeConstructorAccessorImpl.newInstance0(Native Method)
> > at sun.reflect.NativeConstructo