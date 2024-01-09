# 🎈 Pranksters - Aether Interactive

A party game inspired by Ultimate Chicken Horse and Super Mario Party for PC, Mobile, and Console on the Roblox platform built using a TypeScript-to-Luau compiler ([roblox-ts](https://roblox-ts.com)).

<figure><img src="../.gitbook/assets/pranksters.png" alt="" width="563"><figcaption><p>Pranksters Game Page Artwork</p></figcaption></figure>

{% embed url="https://www.roblox.com/games/13943141112/Pranksters-Party-Game" %}
Pranksters Game Page
{% endembed %}

As a gameplay programmer at Aether Interactive, I was apart of a small team creating experiences on the roblox platform. Due to the nature of being in a small team, I was often expected to be more of a generalist programmer and pick up tasks in lots of different areas relating to: Gameplay, UI, , Testing, Networking, Game Design, Sound, Animation, etc.



weekly meetings

code ownership

quick development

game analytics



***

### Key Skills

TypeScript, React Lua, Luau, ESLint

### Key Roblox Libraries

[Flamework](https://fireboltofdeath.dev/docs/flamework/), [Janitor](https://howmanysmall.github.io/Janitor/), [Reflex](https://littensy.github.io/reflex/) (Redux alternative), [Ripple](https://github.com/littensy/ripple), [t](https://github.com/osyrisrblx/t).

<details>

<summary>Full Roblox Libraries (from Package.json)</summary>

```json
"dependencies": {
    "@flamework/components": "^1.0.1",
    "@flamework/core": "^1.0.1",
    "@flamework/networking": "^1.0.1",
    "@gimmethemoney/topbar-plus": "^1.0.3",
    "@rbxts/bezier": "^0.2.0",
    "@rbxts/faker": "^0.2.8",
    "@rbxts/flipper": "^2.0.1",
    "@rbxts/gameanalytics": "2.2.3-ts.1",
    "@rbxts/gizmo": "^2.0.5",
    "@rbxts/inspect": "^1.0.1",
    "@rbxts/janitor": "1.15.4-ts.0",
    "@rbxts/log": "^0.6.3",
    "@rbxts/make": "^1.0.6",
    "@rbxts/message-templates": "^0.3.2",
    "@rbxts/mock-memory-store-service": "0.2.0-13",
    "@rbxts/mockdatastoreservice": "^1.0.2",
    "@rbxts/object-utils": "^1.0.4",
    "@rbxts/pretty-react-hooks": "^0.3.3",
    "@rbxts/profileservice": "^1.4.2",
    "@rbxts/promise-child": "^1.2.1",
    "@rbxts/r15-ragdoll": "github:AetherInteractiveLtd/rbxts-ragdoll",
    "@rbxts/radialimage": "0.1.0-ts.5",
    "@rbxts/rbx-debug": "^1.0.0",
    "@rbxts/rbx-format-number": "^1.0.0",
    "@rbxts/rbx-react-error-boundary": "^1.0.0",
    "@rbxts/rbx-react-spring": "^1.1.2",
    "@rbxts/react-reflex": "^0.2.0",
    "@rbxts/react-roblox": "^0.2.0",
    "@rbxts/reflex": "^4.3.1",
    "@rbxts/ripple": "^0.7.1",
    "@rbxts/roact": "npm:@rbxts/react-ts@^1.0.1",
    "@rbxts/services": "^1.5.1",
    "@rbxts/set-timeout": "^1.1.2",
    "@rbxts/sift": "^0.0.8",
    "@rbxts/signal": "^1.1.1",
    "@rbxts/streamable": "^0.1.0",
    "@rbxts/t": "^3.1.0",
    "@rbxts/validate-tree": "^2.0.2",
    "@rbxts/visualize": "^1.1.1",
    "rbxts-transform-debug": "^2.2.0",
    "rbxts-transform-env": "^2.2.0"
},
"devDependencies": {
    "@milahu/patch-package": "^6.4.14",
    "@rbxts/compiler-types": "2.2.0-types.0",
    "@rbxts/types": "^1.0.738",
    "@roblox-ts/eslint-config": "github:christopher-buss/roblox-ts-eslint-config",
    "@typescript-eslint/eslint-plugin": "^6.17.0",
    "@typescript-eslint/parser": "^6.17.0",
    "cross-env": "^7.0.3",
    "eslint": "npm:eslint-ts-patch@8.56.0-0",
    "eslint-flat-config-viewer": "^0.1.4",
    "eslint-plugin-format": "^0.1.0",
    "eslint-plugin-react": "^7.33.2",
    "eslint-plugin-react-hooks": "^4.6.0",
    "eslint-plugin-sort-class-members": "^1.19.0",
    "eslint-ts-patch": "8.56.0-0",
    "lint-staged": "^15.2.0",
    "prettier": "^3.1.1",
    "rbxts-transformer-flamework": "^1.0.1",
    "rimraf": "^5.0.5",
    "roblox-feet": "^0.0.1",
    "roblox-ts": "^2.2.0",
    "simple-git-hooks": "^2.9.0",
    "typescript": "5.2.2"
},
```

</details>

\[Flamework]\([https://fireboltofdeath.dev/docs/flamework/](https://fireboltofdeath.dev/docs/flamework/)).











\[Flamework]\([https://fireboltofdeath.dev/docs/flamework/](https://fireboltofdeath.dev/docs/flamework/)). \[Flamework]\([https://fireboltofdeath.dev/docs/flamework/](https://fireboltofdeath.dev/docs/flamework/)).

### Technical Skills

1. Knowledge of TypeScript (in a non-web environment), writing type-safe, performant code that
2.



<details>

<summary>React Lua (TypeScript)</summary>

[React Lua](https://github.com/jsdotlua/react-lua) is a comprehensive, but not exhaustive, translation of upstream ReactJS 17.x into Lua. As this project was built using roblox-ts, decleration files were used to type our version of React, making it very similar to the development experience of typical react, but using Roblox elements, rather than HTML.

An example of a file I worked on can be found below:

```typescript
import { useAsyncCallback } from "@rbxts/pretty-react-hooks";
import Roact, { useCallback, useEffect, useMemo, useState } from "@rbxts/roact";

import { Events } from "network/client/network";
import { TextUtil } from "shared/util/text-util";
import { Backplate } from "ui/components/backplate";
import TextButton from "ui/components/buttons/text-button";
import { Group } from "ui/components/group";
import { createNextOrder } from "ui/functions/create-next-order";
import { useRem, useTheme } from "ui/hooks";
import useConfirm from "ui/hooks/use-confirm";

interface Props {
    Position: UDim2;
}

/**
 * A set of buttons that appears in the 'match-over' window, allowing for
 * players to either play again, return to the lobby, or continue with
 * their current session.
 */
export default function InnerButtonBar({ Position }: Readonly<Props>): Roact.Element {
    const confirm = useConfirm();
    const nextOrder = createNextOrder();
    const rem = useRem();
    const theme = useTheme();

    const [isContinue, setIsContinue] = useState(false);

    const allText = useMemo(() => {
        return ["Play Again", "Continue", "Return to lobby"];
    }, []);

    const buttonWidth = rem(10);

    const [textSize, setTextSize] = useState(0);
    useEffect(() => {
        setTextSize(TextUtil.getMaxTextSize(allText, theme.fonts.primary.bold, buttonWidth));
    }, [allText, buttonWidth, rem, theme.fonts.primary.bold]);

    const [, handleBackToLobby] = useAsyncCallback(async (): Promise<void> => {
        const choice = await confirm({
            ConfirmationText: "Are you sure you want to return to lobby?",
        });

        if (choice) {
            Events.requestReturnToLobby.fire(false, false);
        }
    });

    return (
        <Backplate Position={Position} Size={new UDim2(0, rem(40), 0, rem(8.5))}>
            <Group key="buttons" Size={new UDim2(1, 1, 1, 1)}>
                <uilistlayout
                    key="layout"
                    FillDirection="Horizontal"
                    HorizontalAlignment="Center"
                    SortOrder="LayoutOrder"
                    VerticalAlignment="Center"
                />

                <TextButton
                    key="play-again"
                    BackgroundColor={Color3.fromRGB(93, 255, 23)}
                    LayoutOrder={nextOrder()}
                    Text={allText[0]}
                    TextSize={textSize}
                    onClick={useCallback(() => {
                        Events.requestReturnToLobby(true, false);
                    }, [])}
                />

                <TextButton
                    key="continue"
                    BackgroundColor={Color3.fromRGB(255, 216, 20)}
                    Enabled={false}
                    LayoutOrder={nextOrder()}
                    Text={isContinue ? "Waiting..." : allText[1]}
                    TextSize={textSize}
                    onClick={useCallback(() => {
                        setIsContinue(true);
                        Events.requestReturnToLobby(false, true);
                    }, [])}
                />

                <TextButton
                    key="return"
                    BackgroundColor={Color3.fromRGB(69, 215, 255)}
                    LayoutOrder={nextOrder()}
                    Text={allText[2]}
                    TextSize={textSize}
                    onClick={useCallback(async () => {
                        return handleBackToLobby();
                    }, [handleBackToLobby])}
                />
            </Group>
        </Backplate>
    );
}

```

</details>

