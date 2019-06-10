<template>
    <Page>
        <ActionBar title="Welcome to NativeScript-Vue!" android:flat="true"/>
        <TabView android:tabBackgroundColor="#53ba82"
                 android:tabTextColor="#c4ffdf"
                 android:selectedTabTextColor="#ffffff"
                 androidSelectedTabHighlightColor="#ffffff">
            <TabViewItem title="Home">
                <GridLayout columns="*" rows="*">
                    <Label class="message" :text="msg" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="Chat">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Chat" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="Search">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Search" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="Notifications">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="Notifications" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
            <TabViewItem title="User">
                <GridLayout columns="*" rows="*">
                    <Label class="message" text="User" col="0" row="0"/>
                </GridLayout>
            </TabViewItem>
        </TabView>
    </Page>
</template>

<script >
  export default {
    data() {
      return {
        msg: 'Welcome to Home!'
      }
    }
  }
</script>

<style scoped>
    ActionBar {
        background-color: #53ba82;
        color: #ffffff;
    }

    .message {
        vertical-align: center;
        text-align: center;
        font-size: 20;
        color: #333333;
    }
</style>
