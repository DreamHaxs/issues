# ChangeLog
This is the offical github for Depression Hacked Client changelogs & issues

# Macro Tutorial
* Add the Depression.jar as a dependency.

```java
public class Bhop extends Macro {

    public Bhop() {
        super("Bhop", ActivationType.KEY_HELD, Keyboard.KEY_SPACE);
    }

    @Override
    public void onEvent(Event event) {
        if (event instanceof MoveEvent) {
            MoveEvent moveEvent = (MoveEvent) event;
            if (!mc.getPlayer().isPlayerMoving() || mc.getPlayer().isInLiquid())
                return;
            if (mc.getPlayer().isOnGround()) {
                moveEvent.getMotion().setY(0.42F);
                mc.getPlayer().getMotion().setY(0.42F);
                moveEvent.setMovementSpeed(mc.getPlayer().getMovementSpeed() * 2);
            }
        }
    }

    @Override
    public List<Class<?>> classPool() {
        List<Class<?>> classes = new ArrayList<>();
        classes.add(MoveEvent.class);
        return classes;
    }

}
```
* Download: [Test Bhop Macro](https://depressionclient.ml/assets/macros/bhop-macro.jar)
* After that you drag the macro in the macros folder (.minecraft/Depression/macros)

# Depression 1.6 Changelog ( Not out yet )
* Added NoHurtCam

# Depression 1.5 Changelog
* Added an expand scaffold
* Added HypixelHop
* Added Smoothing to Aura
* Recoded RayCast
* Recoded TabGui
* Added Chams
* Fixed Nametags
* Made ChestESP better
* Improvments to Ambiance
* Added a new fly mode for hypixel
* Added Mineplex speed
* Added DAC Hop
* Added DAC OnGround
* Added DAC Fly
* Added DAC Glide up fly
* Added more insults to killsult
* Added BlockHit Module
* Added custom blockit mode
* Added Smoothing in killaura
* Fixed AutoHeal Bug with invalid hotbar selection
* Updated ChestSteal delay in preset command for hypixel
* Added Hypixel NoFall to hypixel preset
* Added a new Hypixel Longjump (Hypixel2)
* Added a DAC LongJump
* Recoded TabGui
* Added a info hud when tabgui is not used

# Depression 1.4 Changelog
* New Bypassing Hypixel Fly
* Added AutoBlock (working on Hypixel)
* Added KillSult Module
* Added Bypassing Hypixel NoFall
* Added Boost To Scaffold
* Added OnGround Hypixel Speed
* Changed .preset Hypixel
* Added Command Predictions
* Fixed alot of bugs
* Added Chat Bypass Module
* Added AutoDisable To Killaura And ChestStealer
* Added PlayerInfo To Killaura
* Added Mineplex Antibot
* Changed Killaura Rotations
* Added .vclip Command
* Added Only Chests Option To ChesStealer Module
* Added Option To Inventory Cleaner So It Does Not Turn Off
* Added Macros
* Added A box above the player that you are hitting with killaura
* Added FionaPort
* Added SpartanHop
* Added NoGround NoFall
* Added ThridPerson Player Model Rotation
* Added Hypixel LongJump
* Made Hypixel Fly Faster
* Fixed a clickgui bug
* Added Depression Capes to Developers
* Added Latest Version Checker
* Added Hypixel Crits
* Added Sneak With 2 Modes (Spoof & Normal)
* Added A Tick Aura (Bypasses Hypixel)
* Fixed a bug with scaffold not switching to original slot when disabled
