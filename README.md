```
local arsenal = require('arsenal');

local function attack(target)
    arsenal.weapon(target).attack();
end

local function reload()
    arsenal.reload();
end

local function target(x, y)
    arsenal.target(x, y);
end

local function shoot()
    arsenal.weapon().shoot();
end

local function reload_all()
    arsenal.reload_all();
end

local function set_target(x, y)
    arsenal.target(x, y, true);
end

local function shoot_all()
    arsenal.weapon_all().shoot();
end

local function aim()
    arsenal.aim();
end

local function shoot_aim()
    arsenal.weapon_aim().shoot();
end

local function reload_aim()
    arsenal.weapon_aim().reload();
end

local function set_mode(mode)
    arsenal.mode(mode);
end

local function set_direction(direction)
    arsenal.direction(direction);
end

local function set_position(x, y)
    arsenal.position(x, y);
end

local function set_health(health)
    arsenal.health(health);
end

local function update()
    arsenal.update();
esp blue color
```
