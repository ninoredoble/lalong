import React from 'react';
import { StyleSheet, Text, View, Image, TextInput } from 'react-native';
import { Provider, IconButton } from 'react-native-paper';

export default function App() {
  return (
    <Provider>
      <View style={styles.container}>
        <View style={styles.header}>
          <IconButton icon="arrow-left" size={24} color="black" />
          <Text style={styles.headerText}>
            <IconButton style={styles.headerIcon} icon="account" size={24} color="black" /> Profile
          </Text>
          <IconButton icon="bell" size={24} color="black" />
        </View>

        <View style={styles.profileSection}>
          <Image source={require('./assets/avatar.png')} style={styles.avatar} />
          <Text style={styles.profileName}>
            G. Niño Emmanuel G. Redoble <IconButton icon="check-circle" size={18} color="black" />
          </Text>
          <View style={styles.followButton}>
            <IconButton icon="plus" size={24} color="black" />
            <Text style={styles.followText}>Follow</Text>
          </View>
        </View>

        <View style={styles.stats}>
          <View style={styles.statItem}>
            <Text style={styles.statNumber}>0</Text>
            <Text style={styles.statTitle}>Clients</Text>
            <Text style={styles.statSubtitle}>Managed</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statNumber}>0</Text>
            <Text style={styles.statTitle}>Projects</Text>
            <Text style={styles.statSubtitle}>Deployed</Text>
          </View>
          <View style={styles.statItem}>
            <Text style={styles.statNumber}>0</Text>
            <Text style={styles.statTitle}>Years</Text>
            <Text style={styles.statSubtitle}>Experienced</Text>
          </View>
        </View>

        <View style={styles.actionButtons}>
          <View style={styles.button}>
            <IconButton icon="account-edit" size={24} color="grey" />
            <Text style={styles.buttonText}>Edit Profile</Text>
          </View>
          <View style={styles.button}>
            <IconButton icon="bell" size={24} color="grey" />
            <Text style={styles.buttonText}>Notifications</Text>
          </View>
          <View style={styles.button}>
            <IconButton icon="account-cog" size={24} color="grey" />
            <Text style={styles.buttonText}>Account Settings</Text>
          </View>
        </View>

        <TextInput style={styles.input} placeholder="Say Something..." placeholderTextColor="#6650A4" />
        <View style={styles.subscribeButton}>
          <IconButton icon="send" size={24} color="grey" />
          <Text style={styles.buttonText}>Subscribe</Text>
        </View>
      </View>
    </Provider>
  );
}

const styles = StyleSheet.create({
  container: { 
    flex: 1, 
    backgroundColor: '#fff', 
    alignItems: 'center', 
    justifyContent: 'center' 
  },
});

{/*

  header: { 
    flexDirection: 'row', 
    justifyContent: 'space-between', 
    alignItems: 'center', 
  },
  headerText: { 
    textAlign: 'center', 
  },
  profileSection: { 
    alignItems: 'center', 
  },
  avatar: { 

  },
  profileName: { 

  },
  followButton: { 
    flexDirection: 'row', 
    alignItems: 'center', 
  },
  followText: { 

  },
  stats: { 
    flexDirection: 'row',   
  },
  statItem: { 
    alignItems: 'center', 
    marginHorizontal: 0, 
  },
  actionButtons: { 
    flexDirection: 'row', 
    justifyContent: 'space-between', 
  },
  button: { 
    flexDirection: 'row', 
    alignItems: 'center', 
  },
  subscribeButton: { 
    flexDirection: 'row', 
    alignItems: 'center', 
  },
  buttonText: { 
    textAlign: 'center' 
  },
  input: { 
  
  },
});

*/}