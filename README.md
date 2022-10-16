# Crashlog
---- Minecraft Crash Report ----
// Daisy, daisy...

Time: 2022-10-16 09:29:18
Description: Rendering item

com.google.common.util.concurrent.ExecutionError: java.lang.NoSuchMethodError: 'boolean net.minecraft.client.renderer.block.model.BakedQuad.hasAmbientOcclusion()'
	at com.google.common.cache.LocalCache$Segment.get(LocalCache.java:2053) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache.get(LocalCache.java:3966) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$LocalManualCache.get(LocalCache.java:4863) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.getBakedInnerModelFor(MateriallyTexturedBakedModel.java:228) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.lambda$getRenderPasses$3(MateriallyTexturedBakedModel.java:188) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at java.util.stream.ReferencePipeline$3$1.accept(ReferencePipeline.java:197) ~[?:?] {}
	at java.util.stream.DistinctOps$1$2.accept(DistinctOps.java:174) ~[?:?] {}
	at java.util.stream.ReferencePipeline$3$1.accept(ReferencePipeline.java:197) ~[?:?] {}
	at java.util.Collections$2.tryAdvance(Collections.java:4853) ~[?:?] {}
	at java.util.Collections$2.forEachRemaining(Collections.java:4861) ~[?:?] {}
	at java.util.stream.AbstractPipeline.copyInto(AbstractPipeline.java:509) ~[?:?] {}
	at java.util.stream.AbstractPipeline.wrapAndCopyInto(AbstractPipeline.java:499) ~[?:?] {}
	at java.util.stream.ForEachOps$ForEachOp.evaluateSequential(ForEachOps.java:150) ~[?:?] {}
	at java.util.stream.ForEachOps$ForEachOp$OfRef.evaluateSequential(ForEachOps.java:173) ~[?:?] {}
	at java.util.stream.AbstractPipeline.evaluate(AbstractPipeline.java:234) ~[?:?] {}
	at java.util.stream.ReferencePipeline.forEach(ReferencePipeline.java:596) ~[?:?] {}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.getRenderPasses(MateriallyTexturedBakedModel.java:189) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115143_(ItemRenderer.java:187) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115127_(ItemRenderer.java:452) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174235_(ItemRenderer.java:507) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174277_(ItemRenderer.java:495) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115218_(ItemRenderer.java:485) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at mezz.jei.common.render.ItemStackRenderer.render(ItemStackRenderer.java:41) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.ItemStackRenderer.render(ItemStackRenderer.java:25) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredient(IngredientListRenderer.java:118) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredientType(IngredientListRenderer.java:98) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.render(IngredientListRenderer.java:88) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGrid.draw(IngredientGrid.java:143) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGridWithNavigation.draw(IngredientGridWithNavigation.java:184) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientListOverlay.drawScreen(IngredientListOverlay.java:188) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.GuiEventHandler.onDrawBackgroundPost(GuiEventHandler.java:60) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.forge.startup.EventRegistration.lambda$registerGuiHandler$12(EventRegistration.java:99) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.core.util.WeakConsumer.accept(WeakConsumer.java:17) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at net.minecraftforge.eventbus.EventBus.doCastFilter(EventBus.java:260) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.lambda$addListener$11(EventBus.java:252) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraft.client.gui.screens.Screen.m_96558_(Screen.java:444) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.Screen.m_7333_(Screen.java:438) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.inventory.InventoryScreen.m_6305_(InventoryScreen.java:74) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraftforge.client.ForgeHooksClient.drawScreenInternal(ForgeHooksClient.java:440) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at net.minecraftforge.client.ForgeHooksClient.drawScreen(ForgeHooksClient.java:433) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at jdk.internal.reflect.GeneratedMethodAccessor16.invoke(Unknown Source) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.optifine.reflect.Reflector.callVoid(Reflector.java:683) ~[OptiFine-1.19.2_HD_U_I1_pre2.jar%23211!/:?] {re:classloading}
	at net.minecraft.client.renderer.GameRenderer.m_109093_(GameRenderer.java:1312) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:securitycraft.mixins.json:camera.GameRendererMixin,pl:mixin:A}
	at net.minecraft.client.Minecraft.m_91383_(Minecraft.java:1115) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91374_(Minecraft.java:700) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.m_239872_(Main.java:212) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:51) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$launchService$0(CommonClientLaunchHandler.java:27) ~[fmlloader-1.19.2-43.1.25.jar%2395!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:106) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:77) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) [bootstraplauncher-1.1.2.jar:?] {}
Caused by: java.lang.NoSuchMethodError: 'boolean net.minecraft.client.renderer.block.model.BakedQuad.hasAmbientOcclusion()'
	at net.minecraftforge.client.model.IQuadTransformer.copy(IQuadTransformer.java:95) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at net.minecraftforge.client.model.IQuadTransformer.process(IQuadTransformer.java:41) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at com.ldtteam.domumornamentum.client.model.baked.RetexturedBakedModelBuilder.lambda$retexture$3(RetexturedBakedModelBuilder.java:127) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at java.util.Optional.map(Optional.java:260) ~[?:?] {re:mixin}
	at com.ldtteam.domumornamentum.client.model.baked.RetexturedBakedModelBuilder.retexture(RetexturedBakedModelBuilder.java:125) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at com.ldtteam.domumornamentum.client.model.baked.RetexturedBakedModelBuilder.lambda$build$0(RetexturedBakedModelBuilder.java:93) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at java.util.ArrayList.forEach(ArrayList.java:1511) ~[?:?] {re:computing_frames,re:mixin}
	at com.ldtteam.domumornamentum.client.model.baked.RetexturedBakedModelBuilder.build(RetexturedBakedModelBuilder.java:90) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.lambda$getBakedInnerModelFor$5(MateriallyTexturedBakedModel.java:240) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at com.google.common.cache.LocalCache$LocalManualCache$1.load(LocalCache.java:4868) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$LoadingValueReference.loadFuture(LocalCache.java:3533) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$Segment.loadSync(LocalCache.java:2282) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$Segment.lockedGetOrLoad(LocalCache.java:2159) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$Segment.get(LocalCache.java:2049) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	... 63 more


A detailed walkthrough of the error, its code path and all known details is as follows:
---------------------------------------------------------------------------------------

-- Head --
Thread: Render thread
Stacktrace:
	at com.google.common.cache.LocalCache$Segment.get(LocalCache.java:2053) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache.get(LocalCache.java:3966) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.google.common.cache.LocalCache$LocalManualCache.get(LocalCache.java:4863) ~[guava-31.0.1-jre.jar%23115!/:?] {}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.getBakedInnerModelFor(MateriallyTexturedBakedModel.java:228) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.lambda$getRenderPasses$3(MateriallyTexturedBakedModel.java:188) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at java.util.stream.ReferencePipeline$3$1.accept(ReferencePipeline.java:197) ~[?:?] {}
	at java.util.stream.DistinctOps$1$2.accept(DistinctOps.java:174) ~[?:?] {}
	at java.util.stream.ReferencePipeline$3$1.accept(ReferencePipeline.java:197) ~[?:?] {}
	at java.util.Collections$2.tryAdvance(Collections.java:4853) ~[?:?] {}
	at java.util.Collections$2.forEachRemaining(Collections.java:4861) ~[?:?] {}
	at java.util.stream.AbstractPipeline.copyInto(AbstractPipeline.java:509) ~[?:?] {}
	at java.util.stream.AbstractPipeline.wrapAndCopyInto(AbstractPipeline.java:499) ~[?:?] {}
	at java.util.stream.ForEachOps$ForEachOp.evaluateSequential(ForEachOps.java:150) ~[?:?] {}
	at java.util.stream.ForEachOps$ForEachOp$OfRef.evaluateSequential(ForEachOps.java:173) ~[?:?] {}
	at java.util.stream.AbstractPipeline.evaluate(AbstractPipeline.java:234) ~[?:?] {}
	at java.util.stream.ReferencePipeline.forEach(ReferencePipeline.java:596) ~[?:?] {}
	at com.ldtteam.domumornamentum.client.model.baked.MateriallyTexturedBakedModel.getRenderPasses(MateriallyTexturedBakedModel.java:189) ~[domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar%23167!/:1.19-1.0.64-ALPHA] {re:classloading}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115143_(ItemRenderer.java:187) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115127_(ItemRenderer.java:452) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174235_(ItemRenderer.java:507) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174277_(ItemRenderer.java:495) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115218_(ItemRenderer.java:485) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at mezz.jei.common.render.ItemStackRenderer.render(ItemStackRenderer.java:41) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
-- Item being rendered --
Details:
	Item Type: vanilla_trapdoors_compat
	Item Damage: 0
	Item NBT: {textureData:{},type:"FULL"}
	Item Foil: false
Stacktrace:
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174235_(ItemRenderer.java:507) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_174277_(ItemRenderer.java:495) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at net.minecraft.client.renderer.entity.ItemRenderer.m_115218_(ItemRenderer.java:485) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default}
	at mezz.jei.common.render.ItemStackRenderer.render(ItemStackRenderer.java:41) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.ItemStackRenderer.render(ItemStackRenderer.java:25) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredient(IngredientListRenderer.java:118) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredientType(IngredientListRenderer.java:98) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.render(IngredientListRenderer.java:88) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGrid.draw(IngredientGrid.java:143) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGridWithNavigation.draw(IngredientGridWithNavigation.java:184) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientListOverlay.drawScreen(IngredientListOverlay.java:188) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.GuiEventHandler.onDrawBackgroundPost(GuiEventHandler.java:60) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.forge.startup.EventRegistration.lambda$registerGuiHandler$12(EventRegistration.java:99) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.core.util.WeakConsumer.accept(WeakConsumer.java:17) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at net.minecraftforge.eventbus.EventBus.doCastFilter(EventBus.java:260) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.lambda$addListener$11(EventBus.java:252) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraft.client.gui.screens.Screen.m_96558_(Screen.java:444) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.Screen.m_7333_(Screen.java:438) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.inventory.InventoryScreen.m_6305_(InventoryScreen.java:74) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraftforge.client.ForgeHooksClient.drawScreenInternal(ForgeHooksClient.java:440) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at net.minecraftforge.client.ForgeHooksClient.drawScreen(ForgeHooksClient.java:433) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at jdk.internal.reflect.GeneratedMethodAccessor16.invoke(Unknown Source) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.optifine.reflect.Reflector.callVoid(Reflector.java:683) ~[OptiFine-1.19.2_HD_U_I1_pre2.jar%23211!/:?] {re:classloading}
	at net.minecraft.client.renderer.GameRenderer.m_109093_(GameRenderer.java:1312) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:securitycraft.mixins.json:camera.GameRendererMixin,pl:mixin:A}
	at net.minecraft.client.Minecraft.m_91383_(Minecraft.java:1115) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91374_(Minecraft.java:700) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.m_239872_(Main.java:212) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:51) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$launchService$0(CommonClientLaunchHandler.java:27) ~[fmlloader-1.19.2-43.1.25.jar%2395!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:106) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:77) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) [bootstraplauncher-1.1.2.jar:?] {}


-- Ingredient being rendered --
Details:
	Mod Name: Domum Ornamentum
	Registry Name: domum_ornamentum:vanilla_trapdoors_compat
	Display Name: Oak Planks Trapdoor
	String Name: 1 vanilla_trapdoors_compat
Stacktrace:
	at mezz.jei.common.util.ErrorUtil.createRenderIngredientException(ErrorUtil.java:158) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredient(IngredientListRenderer.java:122) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.renderIngredientType(IngredientListRenderer.java:98) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.render.IngredientListRenderer.render(IngredientListRenderer.java:88) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGrid.draw(IngredientGrid.java:143) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientGridWithNavigation.draw(IngredientGridWithNavigation.java:184) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.overlay.IngredientListOverlay.drawScreen(IngredientListOverlay.java:188) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.common.gui.GuiEventHandler.onDrawBackgroundPost(GuiEventHandler.java:60) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.forge.startup.EventRegistration.lambda$registerGuiHandler$12(EventRegistration.java:99) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at mezz.jei.core.util.WeakConsumer.accept(WeakConsumer.java:17) ~[jei-1.19.2-forge-11.3.0.262.jar%23176!/:11.3.0.262] {re:classloading}
	at net.minecraftforge.eventbus.EventBus.doCastFilter(EventBus.java:260) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.lambda$addListener$11(EventBus.java:252) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:315) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraftforge.eventbus.EventBus.post(EventBus.java:296) ~[eventbus-6.0.3.jar%2379!/:?] {}
	at net.minecraft.client.gui.screens.Screen.m_96558_(Screen.java:444) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.Screen.m_7333_(Screen.java:438) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:computing_frames,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,xf:fml:configured:set_background_texture_2,pl:mixin:APP:balm.mixins.json:ScreenAccessor,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.gui.screens.inventory.InventoryScreen.m_6305_(InventoryScreen.java:74) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:accesstransformer:B,pl:runtimedistcleaner:A}
	at net.minecraftforge.client.ForgeHooksClient.drawScreenInternal(ForgeHooksClient.java:440) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at net.minecraftforge.client.ForgeHooksClient.drawScreen(ForgeHooksClient.java:433) ~[forge-1.19.2-43.1.25-universal.jar%23202!/:?] {re:classloading}
	at jdk.internal.reflect.GeneratedMethodAccessor16.invoke(Unknown Source) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.optifine.reflect.Reflector.callVoid(Reflector.java:683) ~[OptiFine-1.19.2_HD_U_I1_pre2.jar%23211!/:?] {re:classloading}
	at net.minecraft.client.renderer.GameRenderer.m_109093_(GameRenderer.java:1312) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,xf:OptiFine:default,re:classloading,pl:accesstransformer:B,xf:OptiFine:default,pl:mixin:APP:securitycraft.mixins.json:camera.GameRendererMixin,pl:mixin:A}
	at net.minecraft.client.Minecraft.m_91383_(Minecraft.java:1115) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.Minecraft.m_91374_(Minecraft.java:700) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:mixin,pl:accesstransformer:B,pl:runtimedistcleaner:A,re:classloading,pl:accesstransformer:B,pl:mixin:APP:bookshelf.common.mixins.json:client.AccessorMinecraft,pl:mixin:APP:balm.mixins.json:MinecraftMixin,pl:mixin:APP:playerrevive.mixins.json:MinecraftAccessor,pl:mixin:APP:securitycraft.mixins.json:camera.MinecraftMixin,pl:mixin:A,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.m_239872_(Main.java:212) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at net.minecraft.client.main.Main.main(Main.java:51) ~[client-1.19.2-20220805.130853-srg.jar%23197!/:?] {re:classloading,pl:runtimedistcleaner:A}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke0(Native Method) ~[?:?] {}
	at jdk.internal.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:77) ~[?:?] {}
	at jdk.internal.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43) ~[?:?] {}
	at java.lang.reflect.Method.invoke(Method.java:568) ~[?:?] {}
	at net.minecraftforge.fml.loading.targets.CommonClientLaunchHandler.lambda$launchService$0(CommonClientLaunchHandler.java:27) ~[fmlloader-1.19.2-43.1.25.jar%2395!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandlerDecorator.launch(LaunchServiceHandlerDecorator.java:30) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:53) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.LaunchServiceHandler.launch(LaunchServiceHandler.java:71) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.run(Launcher.java:106) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.Launcher.main(Launcher.java:77) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:26) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.modlauncher.BootstrapLaunchConsumer.accept(BootstrapLaunchConsumer.java:23) [modlauncher-10.0.8.jar%2382!/:?] {}
	at cpw.mods.bootstraplauncher.BootstrapLauncher.main(BootstrapLauncher.java:141) [bootstraplauncher-1.1.2.jar:?] {}


-- JEI render details --
Details:
	Unique Id (for Blacklist): domum_ornamentum:vanilla_trapdoors_compat
	Ingredient Type: class net.minecraft.world.item.ItemStack
	Error Info: 1 vanilla_trapdoors_compat domum_ornamentum:vanilla_trapdoors_compat nbt:{textureData:{},type:"FULL"}

-- Screen render details --
Details:
	Screen name: net.minecraft.client.gui.screens.inventory.InventoryScreen
	Mouse location: Scaled: (310, 230). Absolute: (620.000000, 460.000000)
	Screen size: Scaled: (463, 265). Absolute: (925, 530). Scale factor of 2.000000

-- Affected level --
Details:
	All players: 2 total; [LocalPlayer['AsperOkami'/901, l='ClientLevel', x=160.02, y=64.00, z=102.14], RemotePlayer['Marillo__'/1199, l='ClientLevel', x=171.66, y=68.00, z=105.76]]
	Chunk stats: 289, 167
	Level dimension: minecraft:overworld
	Level spawn location: World: (0,88,0), Section: (at 0,8,0 in 0,5,0; chunk contains blocks 0,-64,0 to 15,319,15), Region: (0,0; contains chunks 0,0 to 31,31, blocks 0,-64,0 to 511,319,511)
	Level time: 2981034 game time, 1110211 day time
	Server brand: forge
	Server type: Non-integrated multiplayer server

-- Last reload --
Details:
	Reload number: 1
	Reload reason: initial
	Finished: Yes
	Packs: Default, Mod Resources

-- System Details --
Details:
	Minecraft Version: 1.19.2
	Minecraft Version ID: 1.19.2
	Operating System: Windows 10 (amd64) version 10.0
	Java Version: 17.0.3, Microsoft
	Java VM Version: OpenJDK 64-Bit Server VM (mixed mode), Microsoft
	Memory: 1153685344 bytes (1100 MiB) / 4093640704 bytes (3904 MiB) up to 5301600256 bytes (5056 MiB)
	CPUs: 4
	Processor Vendor: GenuineIntel
	Processor Name: Intel(R) Core(TM) i5-4570 CPU @ 3.20GHz
	Identifier: Intel64 Family 6 Model 60 Stepping 3
	Microarchitecture: Haswell (Client)
	Frequency (GHz): 3.19
	Number of physical packages: 1
	Number of physical CPUs: 4
	Number of logical CPUs: 4
	Graphics card #0 name: Intel(R) HD Graphics 4600
	Graphics card #0 vendor: Intel Corporation (0x8086)
	Graphics card #0 VRAM (MB): 1024.00
	Graphics card #0 deviceId: 0x0412
	Graphics card #0 versionInfo: DriverVersion=20.19.15.4963
	Memory slot #0 capacity (MB): 8192.00
	Memory slot #0 clockSpeed (GHz): 1.60
	Memory slot #0 type: DDR3
	Virtual memory max (MB): 16853.54
	Virtual memory used (MB): 11172.90
	Swap memory total (MB): 8771.74
	Swap memory used (MB): 1268.80
	JVM Flags: 9 total; -XX:HeapDumpPath=MojangTricksIntelDriversForPerformance_javaw.exe_minecraft.exe.heapdump -Xss1M -Xmx5051M -XX:+UnlockExperimentalVMOptions -XX:+UseG1GC -XX:G1NewSizePercent=20 -XX:G1ReservePercent=20 -XX:MaxGCPauseMillis=50 -XX:G1HeapRegionSize=32M
	Launched Version: ForgeOptiFine 1.19.2
	Backend library: LWJGL version 3.3.1 build 7
	Backend API: Intel(R) HD Graphics 4600 GL version 3.2.0 - Build 20.19.15.4963, Intel
	Window size: 925x530
	GL Caps: Using framebuffer using OpenGL 3.2
	GL debug messages: 
	Using VBOs: Yes
	Is Modded: Definitely; Client brand changed to 'forge'
	Type: Client (map_client.txt)
	Graphics mode: fancy
	Resource Packs: vanilla, mod_resources
	Current Language: English (US)
	CPU: 4x Intel(R) Core(TM) i5-4570 CPU @ 3.20GHz
	OptiFine Version: OptiFine_1.19.2_HD_U_I1_pre2
	OptiFine Build: 20220919-180220
	Render Distance Chunks: 12
	Mipmaps: 4
	Anisotropic Filtering: 1
	Antialiasing: 0
	Multitexture: false
	Shaders: null
	OpenGlVersion: 3.2.0 - Build 20.19.15.4963
	OpenGlRenderer: Intel(R) HD Graphics 4600
	OpenGlVendor: Intel
	CpuCount: 4
	ModLauncher: 10.0.8+10.0.8+main.0ef7e830
	ModLauncher launch target: forgeclient
	ModLauncher naming: srg
	ModLauncher services: 
		mixin-0.8.5.jar mixin PLUGINSERVICE 
		eventbus-6.0.3.jar eventbus PLUGINSERVICE 
		fmlloader-1.19.2-43.1.25.jar slf4jfixer PLUGINSERVICE 
		fmlloader-1.19.2-43.1.25.jar object_holder_definalize PLUGINSERVICE 
		fmlloader-1.19.2-43.1.25.jar runtime_enum_extender PLUGINSERVICE 
		fmlloader-1.19.2-43.1.25.jar capability_token_subclass PLUGINSERVICE 
		accesstransformers-8.0.4.jar accesstransformer PLUGINSERVICE 
		fmlloader-1.19.2-43.1.25.jar runtimedistcleaner PLUGINSERVICE 
		modlauncher-10.0.8.jar mixin TRANSFORMATIONSERVICE 
		modlauncher-10.0.8.jar OptiFine TRANSFORMATIONSERVICE 
		modlauncher-10.0.8.jar fml TRANSFORMATIONSERVICE 
	FML Language Providers: 
		minecraft@1.0
		lowcodefml@null
		javafml@null
	Mod List: 
		doubledoors_1.19.2-3.5.jar                        |Double Doors                  |doubledoors                   |3.5                 |DONE      |Manifest: NOSIGNATURE
		player-animation-lib-forge-0.4.0-test1.jar        |Player Animator               |playeranimator                |0.4.0-test1         |DONE      |Manifest: NOSIGNATURE
		jei-1.19.2-forge-11.3.0.262.jar                   |Just Enough Items             |jei                           |11.3.0.262          |DONE      |Manifest: NOSIGNATURE
		AttributeFix-Forge-1.19.2-17.1.2.jar              |AttributeFix                  |attributefix                  |17.1.2              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		goblintraders-1.7.3-1.19.jar                      |Goblin Traders                |goblintraders                 |1.7.3               |DONE      |Manifest: NOSIGNATURE
		sophisticatedcore-1.19.2-0.5.13.134.jar           |Sophisticated Core            |sophisticatedcore             |1.19.2-0.5.13.134   |DONE      |Manifest: NOSIGNATURE
		waystones-forge-1.19-11.1.0.jar                   |Waystones                     |waystones                     |11.1.0              |DONE      |Manifest: NOSIGNATURE
		journeymap-1.19.1-5.9.0beta2-forge.jar            |Journeymap                    |journeymap                    |5.9.0beta2          |DONE      |Manifest: NOSIGNATURE
		cookingforblockheads-forge-1.19.2-13.2.3.jar      |CookingForBlockheads          |cookingforblockheads          |13.2.3              |DONE      |Manifest: NOSIGNATURE
		comforts-forge-6.0.2+1.19.2.jar                   |Comforts                      |comforts                      |6.0.2+1.19.2        |DONE      |Manifest: NOSIGNATURE
		citadel-1.12.12-1.19.jar                          |Citadel                       |citadel                       |1.12.12             |DONE      |Manifest: NOSIGNATURE
		alexsmobs-1.20.1.jar                              |Alex's Mobs                   |alexsmobs                     |1.20.1              |DONE      |Manifest: NOSIGNATURE
		artifacts-1.19.2-5.0.1.jar                        |Artifacts                     |artifacts                     |1.19.2-5.0.1        |DONE      |Manifest: NOSIGNATURE
		configured-2.0.1-1.19.2.jar                       |Configured                    |configured                    |2.0.1               |DONE      |Manifest: NOSIGNATURE
		DungeonCrawl-1.19-2.3.11.jar                      |Dungeon Crawl                 |dungeoncrawl                  |2.3.11              |DONE      |Manifest: NOSIGNATURE
		Bookshelf-Forge-1.19.2-16.1.5.jar                 |Bookshelf                     |bookshelf                     |16.1.5              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		sophisticatedbackpacks-1.19.2-3.18.29.719.jar     |Sophisticated Backpacks       |sophisticatedbackpacks        |1.19.2-3.18.29.719  |DONE      |Manifest: NOSIGNATURE
		buildinggadgets-3.16.0-build.14+mc1.19.2.jar      |Building Gadgets              |buildinggadgets               |3.16.0-build.14+mc1.|DONE      |Manifest: NOSIGNATURE
		DarkUtilities-Forge-1.19.2-13.1.2.jar             |DarkUtilities                 |darkutils                     |13.1.2              |DONE      |Manifest: NOSIGNATURE
		balm-4.5.3.jar                                    |Balm                          |balm                          |4.5.3               |DONE      |Manifest: NOSIGNATURE
		carryon-1.19-1.18.1.2.jar                         |Carry On                      |carryon                       |1.18.1.2            |DONE      |Manifest: NOSIGNATURE
		forge-1.19.2-43.1.25-universal.jar                |Forge                         |forge                         |43.1.25             |DONE      |Manifest: 84:ce:76:e8:45:35:e4:0e:63:86:df:47:59:80:0f:67:6c:c1:5f:6e:5f:4d:b3:54:47:1a:9f:7f:ed:5e:f2:90
		tl_skin_cape_forge_1.19_1.19.2-1.28.jar           |TLSkinCape                    |tlskincape                    |1.28                |DONE      |Manifest: 19:f5:ce:44:81:0c:e4:22:05:5e:73:c5:a8:cd:de:f3:c8:cf:a9:b3:01:70:40:a0:ee:2d:50:7a:1c:3d:1c:8a
		refinedstorage-1.11.0.jar                         |Refined Storage               |refinedstorage                |1.11.0              |DONE      |Manifest: NOSIGNATURE
		emotecraft-for-MC1.19.2-2.2.5-forge.jar           |Emotecraft                    |emotecraft                    |2.2.5               |DONE      |Manifest: NOSIGNATURE
		ironchest-1.19.2-14.2.7.jar                       |Iron Chests                   |ironchest                     |1.19.2-14.2.7       |DONE      |Manifest: NOSIGNATURE
		client-1.19.2-20220805.130853-srg.jar             |Minecraft                     |minecraft                     |1.19.2              |DONE      |Manifest: a1:d4:5e:04:4f:d3:d6:e0:7b:37:97:cf:77:b0:de:ad:4a:47:ce:8c:96:49:5f:0a:cf:8c:ae:b2:6d:4b:8a:3f
		mcw-bridges-2.0.5-mc1.19.2forge.jar               |Macaw's Bridges               |mcwbridges                    |2.0.5               |DONE      |Manifest: NOSIGNATURE
		voicechat-forge-1.19.2-2.3.10.jar                 |Simple Voice Chat             |voicechat                     |1.19.2-2.3.10       |DONE      |Manifest: NOSIGNATURE
		TerraBlender-forge-1.19.2-2.0.1.127.jar           |TerraBlender                  |terrablender                  |2.0.1.127           |DONE      |Manifest: NOSIGNATURE
		BiomesOPlenty-1.19.2-17.1.1.150.jar               |Biomes O' Plenty              |biomesoplenty                 |17.1.1.150          |DONE      |Manifest: NOSIGNATURE
		NoChatReports-FORGE-1.19.2-v1.4.0.jar             |No Chat Reports               |nochatreports                 |1.19.2-v1.4.0       |DONE      |Manifest: NOSIGNATURE
		Jade-1.19.1-forge-8.3.0.jar                       |Jade                          |jade                          |8.3.0               |DONE      |Manifest: NOSIGNATURE
		CreativeCore_FORGE_v2.8.6_mc1.19.2.jar            |CreativeCore                  |creativecore                  |2.8.6               |DONE      |Manifest: NOSIGNATURE
		spectrelib-forge-0.10.0+1.19.jar                  |SpectreLib                    |spectrelib                    |0.10.0+1.19         |DONE      |Manifest: NOSIGNATURE
		domum_ornamentum-1.19-1.0.64-ALPHA-universal.jar  |Domum Ornamentum              |domum_ornamentum              |1.19-1.0.64-ALPHA   |DONE      |Manifest: NOSIGNATURE
		curios-forge-1.19.2-5.1.1.0.jar                   |Curios API                    |curios                        |1.19.2-5.1.1.0      |DONE      |Manifest: NOSIGNATURE
		reliquary-1.19.2-2.0.20.1166.jar                  |Reliquary                     |reliquary                     |1.19.2-2.0.20.1166  |DONE      |Manifest: NOSIGNATURE
		blockui-1.19-0.0.64-ALPHA.jar                     |UI Library Mod                |blockui                       |1.19-0.0.64-ALPHA   |DONE      |Manifest: NOSIGNATURE
		collective-1.19.2-5.0.jar                         |Collective                    |collective                    |5.0                 |DONE      |Manifest: NOSIGNATURE
		camera-1.19.2-1.0.1.jar                           |Camera Mod                    |camera                        |1.19.2-1.0.1        |DONE      |Manifest: NOSIGNATURE
		PigPen-Forge-1.19.2-11.1.2.jar                    |PigPen                        |pigpen                        |11.1.2              |DONE      |Manifest: NOSIGNATURE
		polymorph-forge-0.45.0+1.19.2.jar                 |Polymorph                     |polymorph                     |0.45.0+1.19.2       |DONE      |Manifest: NOSIGNATURE
		[1.19.2]+SecurityCraft+v1.9.3.1.jar               |SecurityCraft                 |securitycraft                 |1.9.3.1             |DONE      |Manifest: NOSIGNATURE
		FramedBlocks-6.5.0.jar                            |FramedBlocks                  |framedblocks                  |6.5.0               |DONE      |Manifest: NOSIGNATURE
		elevatorid-1.19-1.8.7.jar                         |Elevator Mod                  |elevatorid                    |1.19-1.8.7          |DONE      |Manifest: NOSIGNATURE
		tombstone-8.1.7-1.19.2.jar                        |Corail Tombstone              |tombstone                     |8.1.7               |DONE      |Manifest: NOSIGNATURE
		structurize-1.19.2-1.0.457-ALPHA.jar              |Structurize                   |structurize                   |1.19.2-1.0.457-ALPHA|DONE      |Manifest: NOSIGNATURE
		multi-piston-1.19.2-1.2.19-ALPHA.jar              |Multi-Piston                  |multipiston                   |1.19.2-1.2.19-ALPHA |DONE      |Manifest: NOSIGNATURE
		Runelic-Forge-1.19.2-14.1.2.jar                   |Runelic                       |runelic                       |14.1.2              |DONE      |Manifest: eb:c4:b1:67:8b:f9:0c:db:dc:4f:01:b1:8e:61:64:39:4c:10:85:0b:a6:c4:c7:48:f0:fa:95:f2:cb:08:3a:e5
		minecolonies-1.19.2-1.0.1071-ALPHA.jar            |MineColonies                  |minecolonies                  |1.19.2-1.0.1071-ALPH|DONE      |Manifest: NOSIGNATURE
		cfm-7.0.0-pre34-1.19.jar                          |MrCrayfish's Furniture Mod    |cfm                           |7.0.0-pre34         |DONE      |Manifest: NOSIGNATURE
		CosmeticArmorReworked-1.19.2-v1a.jar              |CosmeticArmorReworked         |cosmeticarmorreworked         |1.19.2-v1a          |DONE      |Manifest: 5e:ed:25:99:e4:44:14:c0:dd:89:c1:a9:4c:10:b5:0d:e4:b1:52:50:45:82:13:d8:d0:32:89:67:56:57:01:53
		expandability-forge-7.0.0.jar                     |ExpandAbility                 |expandability                 |7.0.0               |DONE      |Manifest: NOSIGNATURE
		PlayerRevive_FORGE_v2.0.12_mc1.19.2.jar           |PlayerRevive                  |playerrevive                  |2.0.12              |DONE      |Manifest: NOSIGNATURE
	Crash Report UUID: 5288e933-b3be-4e3e-8ff9-3877bd9a253c
	FML: 43.1
	Forge: net.minecraftforge:43.1.25
	FramedBlocks BlockEntity Warning: Not applicable
